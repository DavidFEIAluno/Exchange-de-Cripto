# Objetivo do Projeto
Criar um código onde seja possível comercializar criptomoedas, juntamente com uma criação de conta, e que seje possível ter mais fácil acesso juntamente com uma boa segurança, para que enfim, avançemos ainda mais para o futuro com essas novas mecânicas e ideias.

# Forma de compilação e execução
Primeiro, salve o arquivo com alguma extensão em C, coloque o nome do arquivo, no meu caso programa_exchange_finalizado.c
para que seje possivel compilar, utilize algum compilador em C.
Se for em Linux/macOS: Abra o terminal e navegue até o diretorio do arquivo, usando por exemplo "cd \caminho\para\o\diretorio" compile o arquivo .c em GCC "gcc programa_exchange_finalizado.c -o" "programa_exchange_finalizado.exe".
já no Windows, "cd C:\caminho\para\o\diretorio" bash: "gcc programa_exchange_finalizado.c -o" "programa_exchange_finalizado.exe
A Execução: 
No Linux/macOS: ./programa_exchange_finalizado
No Windows: programa_exchange_finalizado.exe

# Funções e explicações do código:
Cadastro e Login
Cadastrar usuário: O código permite o cadastro de novos usuários. O CPF e a senha são validados para garantir que estejam no formato correto (No caso respectivamente XXX.XXX.XXX-XX e senha de 6 digitos). Após o cadastro, os dados do usuário são armazenados.
Login: Após o cadastro, o usuário pode realizar o login, onde o CPF e senha são comparados com os dados armazenados. O sistema carrega os usuários de um arquivo binário para verificar as credenciais.
Salvar e carregar usuários: Os dados dos usuários (CPF, saldo, criptomoedas) são salvos em um arquivo binário e carregados quando o programa é iniciado, permitindo que as informações persistam entre sessões.

Operações financeiras
Consultar saldo: O usuário pode visualizar seu saldo em reais e o saldo em criptomoedas (Bitcoin, Ethereum e Ripple).
Depositar reais: Permite ao usuário adicionar saldo em reais à sua conta.
Sacar reais: O usuário pode sacar uma quantia em reais de seu saldo, desde que tenha fundos suficientes (Exemplo, se foi depositado 10 Reais, será impossivel de sacar 11 Reais).
Comprar criptomoedas: O usuário pode comprar criptomoedas (Bitcoin, Ethereum, Ripple) usando seu saldo em reais, contanto que tenha a quantia necessária. As cotações das criptomoedas são atualizadas periodicamente com variações aleatórias.
Vender criptomoedas: O usuário pode vender suas criptomoedas, convertendo-as de volta para reais com base na cotação atual.
Atualizar cotações: As cotações das criptomoedas são ajustadas em um intervalo de -5% a +5% da cotação anterior.
Consultar extrato: O sistema mantém um registro das transações realizadas (como depósitos, saques, compras e vendas de criptomoedas) e permite que o usuário visualize esse histórico.

Menu Principal
Apos o Login ser efetuado, o sistema mostra um Menu com as principais 8 opções ditas anteriormente.
O código lida com três criptomoedas (Bitcoin, Ethereum, Ripple), e suas cotações são ajustadas aleatoriamente em intervalos pré-definidos. O usuário pode realizar transações baseadas nessas cotações.

# Projeto 3

Objetivo do Programa:
O programa implementa um sistema de gerenciamento para investidores e transações financeiras envolvendo criptomoedas. Ele permite funcionalidades como:
Cadastro e exclusão de investidores e criptomoedas.
Consulta de saldo e extrato de transações.
Atualização de cotações de criptomoedas.
Registro de transações financeiras.

Forma de Compilação e Execução:
Compilação: Use um compilador de C, como gcc. Execute o seguinte comando no terminal para compilar o programa:
"gcc programa.c -o programa"
Substitua programa.c pelo nome do arquivo.

Execução: Após a compilação, execute o programa gerado:
./programa

Forma de Uso do Programa:
Ao iniciar, o programa solicita o login do usuário, pedindo o CPF e a senha. Se o login for bem-sucedido, o menu principal é exibido, apresentando opções como:

Cadastrar e excluir investidores.
Adicionar ou remover criptomoedas.
Consultar saldo e extrato de um investidor.
Atualizar as cotações das criptomoedas.
O usuário seleciona uma opção digitando o número correspondente e segue as instruções.
O programa salva os dados de investidores e criptomoedas em arquivos binários para persistência.
Validação de CPF: Assegura que o CPF inserido siga o formato xxx.xxx.xxx-xx.
Persistência de Dados: Os dados de investidores e criptomoedas são salvos em arquivos binários, garantindo que sejam preservados entre as execuções.

Funcionalidades Gerais:
Investidores: É possível cadastrar, consultar saldo/extrato, e excluir investidores.
Criptomoedas: O sistema permite cadastrar novas criptomoedas, excluir existentes e atualizar suas cotações.
Transações: Todas as operações financeiras são registradas com detalhes como tipo, valor e data.
Interface Simples: A interação é baseada em menus numéricos, tornando o programa intuitivo.

Feito Por: David Ivaldi Elhain
RA: 24.124.009-2
Link para o acesso: https://github.com/DavidFEIAluno/Exchange-de-Cripto
