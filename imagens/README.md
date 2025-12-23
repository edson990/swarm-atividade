Pasta para armazenar as imagens 

Nas imagens apresentadas, eu demonstro o funcionamento de uma API executando em um ambiente com Docker Swarm.

Nas respostas da rota /info, é possível observar que a API retorna o status do serviço, o nome do host e o horário da requisição. O nome do host muda entre as requisições, indicando que o Docker Swarm está distribuindo as chamadas entre diferentes containers.

Também é mostrado o resultado do comando docker service ps, onde é possível verificar que o serviço possui várias réplicas ativas. Mesmo quando um container é interrompido, o Swarm mantém o serviço em execução, garantindo a disponibilidade da aplicação.

Esses testes comprovam o funcionamento da redundância e do balanceamento de carga no ambiente configurado.
