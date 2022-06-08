========================== Aula 1 ========================

Siga o guia de instalação da documentação do site
oficial:

https://tailwindcss.com/docs/installation


Toda a estilização proposta pelo Tailwind dentro do próprio
arquivo HTMl através das classes. 


========================== Aula 2 ========================

- Fontes:

    - Tamanho da fonte:
    A classe para a estilização de fontes é a classes
    "text" + "abreviação do tamanho".
    Ex:

    <h1 class"text-sm">Hello World</h1>
    > text small = 0.875rem / 14px
    <h1 class"text-base">Hello World</h1>
    >text base = 1rem / 16px
    <h1 class"text-lg">Hello World</h1>
    >text large = 1.125rem / 18px
    <h1 class"text-xl">Hello World</h1>
    >text extra large = 1.25rem / 20px
    <h1 class"text-5xl">Hello World</h1>
    >text 5x extra large = 3rem/ 30px

    (Para mais tamanhos consultar: https://tailwindcss.com/docs/font-size)


    - Cor da fonte:

    A classe para a cor da fonte é definida por:
    "text" + "nome da cor" + "intensidade da cor"
    Ex:

    <h1 class="text-gray-500">Hello World<h1>
    <h1 class="text-blue-400">Hello World<h1>
    <h1 class="text-green-700">Hello World<h1>

    (Para mais cores consultar: https://tailwindcss.com/docs/text-color)

    
    - Peso da fonte:

    A classe para o peso da fonte é definida por:
    "text" = "peso"
    Ex:

    <h1 class="text-light">Hello World<h1>
    >font-weight: 300
    <h1 class="text-normal">Hello World<h1>
    >font-weight: 400
    <h1 class="text-medium">Hello World<h1>
    >font-weight: 500
    <h1 class="text-bold">Hello World<h1>
    >font-weight: 600

    - Alinhamento de fonte:

    A classe para alinhamento da fonte é:
    "texto" + "propriedade"
    Ex:

    <h1 class="text-left">Hello World<h1>
    >text-align: left
    <h1 class="text-center">Hello World<h1>
    >text-align: center
    <h1 class="text-right">Hello World<h1>
    >text-align: right
    


Para mais estilizações de fontes, consultar:

https://tailwindcss.com/docs -> tipography



========================== Aula 3 ========================


É importante entender e/ou relembrar, as unidades de espa
çamento do CSS.

Basicamente as principais são: rem e pixels:

    1rem = 16px
    1.25rem = 20px

E no tailwind, o valor padrão correspondendo é o número
4, ou seja:

    4 = 16px = 1 rem

Veja alguns exemplos práticos:

-Espaçamentos

   Padding:

   <h1 class="p-2">Hello World<h1>
    >padding = 0.5rem = 8px
    <h1 class="p-4">Hello World<h1>
    >padding = 1rem = 16px
    <h1 class="p-8">Hello World<h1>
    >padding = 2rem = 32px

   É possível fazer selecionado o eixo, desejado. Basta
   selecionar X ou Y:

   <h1 class="px-4">Hello World<h1>
    >padding = 1 rem = 16px (para left e right)
    <h1 class="py-4">Hello World<h1>
    >padding = 1 rem = 16px (para top e bottom)


   Logicamente, também é possível selecionar apenas um lado
   em específico, basta utilizar a regra:

   t = top
   b = bottom
   r = right
   l = left

   ex:

   <h1 class="pt-4">Hello World<h1>
    >padding top = 1rem = 16px

   Margin:

   É o mesmo exemplo, basta substituir o P por M.

   Space-Between

   Devido a recorrencia da necessidade de criar um espaçamento
   entre elementos do HTML, o Tailwind criou um classe para 
   facilitar esse processo. A class é : 
   "space" + "eixo" + "unidade de medida"

   Ex:
   Espaçamento entre itens do eixo x:

   <div class="space-x-4">
      <h1>Hello world</h1>
      <h1>Hello world</h1>
      <h1>Hello world</h1>
   </div>
   >Todos os H1 terão um espaçamento no eixo x de 1rem/16px


Para mais consultar consultar:
https://tailwindcss.com/docs/customizing-spacing



========================== Aula 4 ========================


- Border

    Border Radius

    A classse para border radius formada por:
    "rounded-" + "escala"
    Ex:

    <div class="rounded"></div>
    >border-radius = 0.25rem


    Border Width:

    A classe é formada por:
    "border" + "escala"

    <div class="border"></div>
    >border-width = 1px 
    <div class="border-2"></div>
    >border-width = 2px 


    Border Color:

    A classe border color é formada por:
    "border" + "cor" + "escala"

    <div class="border-green-100"></div>
    >border-color = green
    

(Para mais consultas a respeito de bordas, acesse:
https://tailwindcss.com/docs/border-radius)



========================== Aula 5 ========================


Background

   Background Color
   
   A classe background color é formada por:
   "bg" + "cor" + "escala"

   Ex:
   <div class="bg-green"></div>
    >background-color = green


   Background Image (gradient)

   A classe background img pode ser usada pra criar gradientes.
   Ela é formada por:
   "bg-" - "gradient-to-" "direção". 

   Direções:
   t - cima
   r - direita
   l - esquerda
   b - baixo
   tr - cima direita
   etc.

   Em conjunto com outras classes:
   "from-" + "cor+escala" 
   "via-" + "cor+escala"
   "to-" + "cor+escalda"
   Ex:
   
   <div class="bg-gradient-to-t from-yellow-400 via-red-500 to-pink-500"></div>
   >gradient terá direção ao top 
   >Da cor amarela 400
   >Através da cor vermelha 500
   >Até o pink 500



========================== Aula 6 ========================



Tamanhos de componentes

Width
    O width é formado pela classe:
    "w" + "escala"
    ex:

   <div class="w-4"></div>
   > width = 1rem / 16px

   <div class="w-px"></div>
   > width = 1px

   <div class="w-1/2"></div>
   > width = metade do elemento pai

Max Width
    Para criar uma regra de largura máxima, digite:
    'max" + "w" + "escalda"
    Ex:

   <div class="max-w-1/2"></div>
   > max-width = metade do elemento pai

Min width
    Para criar uma regra de largura mínima, digite:
    "min" + "w" + "escala"


height
    O height segue exatamente a mesma regra e valores
    do width




========================== Aula 7 ========================



Flexbox:

  Para ativar o display flex, digite a classe:
  "flex"
  Ex:

  <div class="flex"></div>
  > display flexbox


  Direction

  Para escolher a direção digite:
  "flex-" + "row" ou "collum"

  Para demais regras do flexbox, utilize a mesma lógica.


  Justify Content

  Para inseri justify, digite a classe:
  "justify-" + "valor"
  ex:

  <div class="flex justify-start"></div>
   > justify-content = elementos ficaram a esquerda dentro do conteúdo pai.



========================== Aula 8 ========================

Aula de Grid

CONSULTAR DOCUMENTAÇÃO


========================== Aula 9 ========================


Responsividade.

Dentro do arquivo tailwind.config.js, cre um objeto de nome "screens", 
dentro do objeto "theme", dentro dele, é possível setar alguns valores
de responsividade com base em pixels. Siga o exemplo:

    'sm': '640px'
    > @media (min-width: 640px)


  Objeto pré criado:

  screens {
      'sm': '640px',
      'md': '768px',
      'lg': '1024px',
      'xl': '1280px',
      '2xl': '1536px'
  }

  Esses parâmetros devem ser usados de prefixo para a classe que sera 
  aplicada para a responsividade.

  Ex:

  <div class="md:text-4"></div>
  > @media (min-width: 640px) {
  >    texto de tamanho 1rem / 16px
  >}


========================== Aula 10 ========================


Estados

Os estados funcionam de forma bem semalhante a media querys. 

  Hover 
  Basta digitar o prefixo "hover:" antes da classe.

  Focus
  Basta digitar o prefixo "focus:" antes da classe.

  Active
  Basta digitar o prefixo "active:" antes da classe

  Group-hover
  Basta digitar o prefixo "grou-hover:" antes da classe

  Ex:
  <div class="hover:text-grey-800 focus:underline"></div>
  > Ao passar o mouse o texto fica cinza, e ao clicar o texto
  > ficará sublinhado.

  Caso vá usar o group, é necessário declar a classe "group"
  no elemento pai.
  Ex:

  <div class="group">
    <div class="group-houver:text-blue-300"></div>
  </div>




========================== Aula 11 ========================


Arquivo de Configuração.

  Como já visto anteriormente, o arquivo tawildin.config.js
  é o arquivo de configuração do tailwind, possibilidante a 
  personalização do mesmo. Há possbilidade de criar suas 
  proprias variáveis e valores, dentre deste mesmo arquivo.


   purge[]

   Este array serve para inibir o carregamento de todo
   o arquivo tailwind, que é muito pesado.

   darkMode:

   valor de true ou false, para o modo noturno.

   theme: {}

   Neste objeto iremos colocar das as classes personalizadas
   criadas por nós.

   extend {}

   Objeto que da a possibilidade de extender as classes bases
   do tailwind


Em caso de dúvidas em como preencher, acesse:

https://tailwindcss.com/docs/configuration
https://www.youtube.com/watch?v=nsMvmjGhG48&list=PLcoYAcR89n-r1m-tMfV4qndrRWpT_rb9u&index=11&ab_channel=TiagoMatos



========================== Aula 12 ========================




   
