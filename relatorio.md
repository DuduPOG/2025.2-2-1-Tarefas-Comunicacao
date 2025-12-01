# Relato da atividade de comunicação entre processos usando sockets

## Informações gerais

- **Disciplina**: Sistemas operacionais

- **Semestre letivo**: 2025.2
- **Aluno**: Eduardo Medeiros de Sousa Aguiar

## Sumário

- [**Parte 1 - 1 servidor e 1 cliente (bloqueante)**](#parte-1--1-servidor-e-1-cliente-bloqueante)

- [**Parte 2 — 1 servidor e 2 clientes (bloqueante)**](#parte-2--1-servidor-e-2-clientes-bloqueante)
- [**Parte 3 — Modificar o servidor para múltiplos clientes**](#parte-3--modificar-o-servidor-para-múltiplos-clientes)
- [**Parte 4 — 1 servidor (concorrente) e 2 clientes**](#parte-4--1-servidor-concorrente-e-2-clientes)

## Parte 1 — 1 servidor e 1 cliente (bloqueante)

### Servidor iniciando e aguardando conexão

```bash
(virtual) PS C:\Users\20242014040005\Documents\ws-so\2025.2-2-1-Tarefas-Comunicacao> python src/servidor.py 
Servidor Echo escutando em localhost:5000

Aguardando conexão...
```

### Cliente se conectando com o Servidor

- **Cliente**

```bash
(virtual) PS C:\Users\20242014040005\Documents\ws-so\2025.2-2-1-Tarefas-Comunicacao> python src/cliente.py  
Conectado ao servidor Echo
Digite "sair" para encerrar a conexão

Digite uma mensagem:   
```

- **Servidor**

```bash
Conectado com ('127.0.0.1', 60257)
```

### Troca de mensagens

- **Cliente**

```bash
Digite "sair" para encerrar a conexão

Digite uma mensagem: oi
Resposta: Echo: oi
```

- **Servidor**

```bash
Recebido: oi
```

### Conexão encerrada limpidamente

- **Cliente**

```bash
Digite uma mensagem: sair
Conexão encerrada
(virtual) PS C:\Users\20242014040005\Documents\ws-so\2025.2-2-1-Tarefas-Comunicacao> 
```

- **Servidor**

```bash
Cliente desconectou

Aguardando conexão...
```

### Observação

O cliente envia uma mensagem e espera recebâ-la de volta através de uma resposta echo e o servidor espera receber uma mensagem do cliente e retorná-la para confirmar o êxito da tarefa.

## Parte 2 — 1 servidor e 2 clientes (bloqueante)

FIXME seu relato

## Parte 3 — Modificar o servidor para múltiplos clientes

FIXME seu relato

## Parte 4 — 1 servidor (concorrente) e 2 clientes

FIXME seu relato
