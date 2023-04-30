</h1>

<img src="https://user-images.githubusercontent.com/104467309/188473729-68d7615b-64dd-4478-b44d-1484b4db4141.png" width="250px"> 

</h1>

# O que é o Cypress e porque preciso dele ?

É uma ferramenta de teste rápido, fácil e confiável para qualquer coisa que seja executada em um navegador, para teste de aceitação ou e2e (end-to-end). Veio com propósito de facilitar o processo de configuração, execução e depuração dos seus testes.

# Não é reinventar a roda!

Cypress não é um framework de automação geral, nem é uma estrutura de teste de unidade para seus serviços de back-end afinal existem ótimas ferramentas por aí que fazem isso. É uma excelente ferramenta que traz uma nova experiência enquanto escreve testes end-to-end para seus aplicativos web.

# Outra ferramenta de teste?

Você deve estar se perguntando "Nossa outra ferramenta de teste, já vi inúmeras e nada resolve meu problema, sempre um mar de configuração e detalhes, será mesmo que devo perder meu tempo?"
Calma jovem realmente existe algo diferente e é bem legal.

## Alguns dos principais pontos do Cypress.io

___________________________________________________________________________
Free e open source.
___________________________________________________________________________
Testes em Javascript.
___________________________________________________________________________
Continuous Integration.
___________________________________________________________________________
Time Travel.
___________________________________________________________________________
Real time reloads.
___________________________________________________________________________
Automatic waiting.
___________________________________________________________________________
Spies, stubs e clocks.
___________________________________________________________________________
Controle do tráfego de rede.
___________________________________________________________________________
Screenshots e vídeos.
___________________________________________________________________________
Testar responsividade em web apps.
___________________________________________________________________________

Alguns desses pontos você já pode ter visto em outras ferramentas mas será mesmo que conseguiu utiliza-lá de maneira fácil e colocar em prática tudo o que a ferramenta prometia? Mais pra frente irei explicar alguns desses pontos.

# Arquitetura e funcionamento

A imagem abaixo mostra um conjunto de ferramentas e tecnologias que foram utilizadas na construção do Cypress.io. Motivo pela qual se torna um instrumento tão poderoso e ao mesmo tempo intuitivo.


</h1> <img src="https://user-images.githubusercontent.com/104467309/235354341-9b847286-b553-4bf9-a3a6-742310506a71.jpg" width="995px">  
   </h1>

# Tudo é simples e intuitivo, veja na imagem baixo o painel de testes.

</h1> <img src="https://user-images.githubusercontent.com/104467309/235356586-b2782e66-8f3d-4153-a0ce-f0cb8b3ed8a6.jpg" width="995px">  
   </h1>
   
# Primeiros passos com Cypress

## Criando setup de testes

Bom, antes de mais nada precisamos baixar as dependencias e instalar o cypress em seu projeto.

Acesse a pasta do seu projeto ou crie uma.

`$ mkdir cypress-example`

Dentro do diretório criado instale o cypress.

`$ npm install cypress --save-dev`

Após a instalação execute o cypress.

`$ ./node_modules/.bin/cypress open`

Após instalação e execução irá notar que será mostrar uma tela com vários testes criados. Na raiz do diretório uma nova pasta cypress e o arquivo cypress.json serão criados.   

</h1> <img src="https://user-images.githubusercontent.com/104467309/235357860-9c3ca3aa-5c78-41e5-b5c0-b972a1bac463.jpg" width="995px">  
   </h1>

Agora já estamos prontos para criar nossos testes. Por padrão Cypress cria alguns testes de exemplo que são úteis inicialmente para visualizar como selecionar um elemento e efetuar uma ação.

# Estrutura de diretórios

Confira dentro da pasta do cypress que existem outros diretórios e que cada um deles tem seu objetivo, veja a imagem abaixo.

</h1> <img src="https://user-images.githubusercontent.com/104467309/235358207-1b6676ad-97ba-476e-b576-11390f61e486.jpg" width="995px">  
   </h1>

- Fixtures: É onde seus mocks são armazenados podendo ser utilizados em qualquer teste.

- Integrations: Aqui é o diretório onde criará seus arquivos de teste exemplo : app_spec.js ou .js .jsx .coffee .cjsx.

- Plugins: Com eles é possível trocar, modificar ou estender o comportamento interno do Cypress.

Exemplos de plugins:

-> Trocar variáveis de ambiente durante o processo de execução

-> Carregar arquivos utilizando a lib fs

- Support: Neste diretório é possível criar comandos que podem ser executados dentro dos testes ou sobrescrever comandos já existentes.
Exemplo de comandos:

-> Comando para login ( Evitar duplicação de código)

-> Comando para logout

# Como aprender a criar testes com Cypress

Para começar a entender como os testes funcionam acesse a pasta integration. Lá vários arquivos de testes com exemplos foram criados. Ao instalar o cypress recomendo que análise os arquivos na pasta integration pois todos eles serão muito úteis como guia.

Há, não esqueça de apertar o play e ver o cypress em ação e executando todos os testes, fique a vontade também pra modificar os arquivos e ver na prática o que acontece.





