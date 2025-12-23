Esse projeto eu fiz pra mostrar como funciona a redundância usando Docker Swarm. Eu criei uma API simples em Node.js e rodei ela com várias réplicas no Swarm. Assim, quando alguém faz uma requisição, o Swarm distribui entre os containers automaticamente.

Pela rota /info dá pra ver qual container respondeu, então fica fácil perceber o balanceamento de carga. Também usei um serviço que fica fazendo requisições direto pra API, pra acompanhar se tudo continua funcionando mesmo quando algum container para.

No fim, o projeto mostra que, mesmo se uma instância cair, a aplicação continua rodando normalmente por causa do Swarm.
