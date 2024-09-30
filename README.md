

Projeto de Locadora de Veículos 

Esse projeto foi desenvolvido em grupo como parte do curso Santander Coders 2024.1 da AdaTech, focando em Programação Orientada a Objetos. Abaixo, uma visão geral das principais classes e funcionalidades.

 Estrutura 

**1. Aluguel**  
- **Classe Aluguel**: Guarda as informações de um aluguel de veículo.
- **Classe AluguelServiceImpl**: Gerencia o processo de aluguel. Pode iniciar o aluguel com a data atual ou uma data específica, verificando a disponibilidade do veículo.

**2. Devolução**  
- **DevolucaoFactory**: Cria a devolução de um veículo. Aplica descontos dependendo se o cliente é pessoa física ou jurídica e utiliza o serviço de devolução correspondente.
- **DevolucaoServiceBase**: Interface para diferentes serviços de devolução.

**3. Cliente**  
- **Classe Cliente**: Armazena os dados do cliente, como nome e documento.
- **ClienteRepositoryInMemoryImpl**: Simula um banco de dados em memória para armazenar, buscar, atualizar e remover clientes.

**4. Repositórios**  
- **CrudRepository**: Interface para criar, ler, atualizar e excluir dados.
- **AgenciaRepository**: Gerencia operações de agência.
- **AgenciaRepositoryInMemoryImpl**: Armazena dados de agências em memória.

**5. Veículo**  
- **Classe Veiculo**: Representa um veículo. Seu gerenciamento (criação, alteração, busca) é feito pelo `VeiculoService`.
- **VeiculoServiceImpl**: Cuida das operações de criar, deletar, alterar e buscar veículos.
- **VeiculoFactory**: Cria novos veículos com base em tipo, placa e modelo.

Funcionalidades da Aplicação



- Cadastrar, alterar e buscar veículos.
- Cadastrar e alterar agências.
- Cadastrar, alterar e buscar clientes.
- Alugar veículos para pessoas físicas e jurídicas.

