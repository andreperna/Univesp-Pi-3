# Univesp-Pi-3 (Projeto Integrador)
Projeto Integrador nº 3 da UNIVESP, referente ao 4º Semestre (Bimestres 7 e 8)

&nbsp;

# Título: Armazenamento de Acúcar: Controle de Estoque de Bags

&nbsp;

## Resumo
Este trabalho tem como objetivo contribuir com o setor Sucroenergético na área de Armazenagem de Bags de Açúcar, visando o desenvolvimento de técnicas avançadas de Controle de Estoque que permitam otimizar ao máximo a Gestão dos Armazéns em tempo real, além disso, estas técnicas permitirão maior rastreabilidade do produto e, consequentemente maior assertividade na tomada de decisões, seja em cenários atuais ou futuros. Atualmente, este controle é feito por meio de anotações manuais em pranchetas, que só estarão disponíveis aos gestores depois de toda contagem ser feita, o que, além de ineficiente, pode apresentar informações imprecisas. Conforme a tecnologia se desenvolve, nota-se uma tendência de automatização de várias tarefas nos vários ramos da sociedade, gerando maior fluxo de informações, que serão cada vez mais precisas. Com este projeto, é esperado que os dados gerados durante a entrada e saída de bags de açúcar sejam mais precisos e que estes cheguem aos gestores em tempo real, melhorando o controle a aumentando a confiabilidade das informações.

&nbsp;

## Prototipação
Atualmente o protótipo está em fase de desenvolvimento, porém já conta com os recursos essenciais para simular a situação problema. Tal situação seria a leitura de dados via QRcode, a fim de controlar a entrada e saída de bags de açúcar nos armazéns. Tal controle é realizado por meio de um aplicativo, que está sendo desenvolvido através do Kodular, um mecanismo online para criação de softwares para smartphones. A linguagem de programação utilizada por esta plataforma é baseada no que se chama linguagem de blocos que, como implícito no nome, permite ao usuário criar a automatizar rotinas computacionais através da concatenação de blocos.
No entanto, é necessário que tais dados sejam armazenados em algum local, pois, a fim de monitorar a eficiência do processo de entrada e saída dos bags, os gestores responsáveis desejarão gerar relatórios e gráficos com o máximo de informações possíveis, como comparativos de um mês para outro. A fim de suprir a demanda de armazenamento de dados à longo prazo, o projeto contará com uma base de dados em um ambiente cloud, chamada Firebase, que receberá as informações provenientes dos QRCodes lidos durante o processo.
O funcionamento do sistema será por meio de uma interface gráfica, na qual sofrerá interação de um usuário, que deverá conter as permissões necessárias para executar as tarefas desejadas. Dos recursos disponíveis no aplicativo, o operador poderá exercer tarefas que seriam realizadas no armazém após o processo de pesagem e identificação (via etiquetas QRCode) dos bags de açúcar, em que ao estarem no armazém, os bags com os produtos serão lidos pelo operador no momento de entrada ou saída. Se não houver erro ou violação no código, os dados do bag serão enviados ao banco de dados, que os armazenará, no caso de entrada de bags. Caso o produto seja lido no momento em que o mesmo será disponível para o comércio, ou seja, no momento da saída, os dados serão enviados ao banco de dados, requisitando o decremento da quantidade de bags em estoque, além de informações referentes à saída do produto.
Além das ferramentas de entrada e saídas de mercadorias, o sistema possui um mecanismo que realiza a leitura dos dados, que também está em desenvolvimento, para que os operadores e os gestores possam verificar as quantidades de bags disponíveis no estoque físico e/ou histórico de todas os registros na base de dados. Tal recurso permite que os gestores tomem decisões no âmbito financeiro ou no próprio processo produtivo, pois, em caso de falta de produtos, os mesmos podem rever todo o processo de produção de açúcar, a fim de identificar possíveis lacunas, e, consequentemente, buscar soluções para tais.
Para atingir os objetivos propostos e o fluxo de trabalho desejado, será construído um sistema de aplicação mobile, que será composto inicialmente por 4 telas:
- **Home**: tela onde estarão disponíveis os botões para adicionar ou retirar itens do armazém, por meio da ativação da câmera do celular e leitura do QRCode.

- **Entradas**: nesta tela serão listadas as entradas do armazém, gerando um histórico para posterior consultas.

- **Saídas**: tela onde serão listadas as saídas do armazém, gerando um histórico para posterior consultas, assim como na tela de entradas.

- **Saldo**: nesta tela pretende-se apresentar, além do saldo atual do estoque, algumas estatísticas de armazenamento, entradas e saídas

## Desenvolvimento do Sistema
O sistema foi desenvolvido na plataforma Kodular, por tratar-se de um ambiente para desenvolvimento mobile, com programação por meio de blocos.

&nbsp;

# Telas do Sistema
- Home
![Home](https://github.com/andreperna/Univesp-Pi-3/blob/master/Prints%20de%20Tela/Home.jpeg?raw=true)

- Entradas
![Entradas](https://github.com/andreperna/Univesp-Pi-3/blob/master/Prints%20de%20Tela/Entradas.jpeg?raw=true)

- Saidas
![Saidas](https://github.com/andreperna/Univesp-Pi-3/blob/master/Prints%20de%20Tela/Saidas.jpeg?raw=true)

- Saldo
![Saldo](https://github.com/andreperna/Univesp-Pi-3/blob/master/Prints%20de%20Tela/Saldo.jpeg?raw=true)

- Menu
![Saldo](https://github.com/andreperna/Univesp-Pi-3/blob/master/Prints%20de%20Tela/Menu.jpeg?raw=true)