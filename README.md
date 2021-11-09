# Crud-Angular-Spring
Primeiro projeto Angular!

##  Criando um projeto Angular

## Rodando a aplicação Angular
- Abrir o projeto no Visual Studio Code 
- Abrir um novo terminal (Terminal > New Terminal) 
- comando 'ng serve' para rodar a aplicação
- Abrir no browser "localhost:4200"

## Instalando Angular Material
- No terminal digitar  o comando 'ng add @angular/material' para instalar o angular material
- Ira perguntar se você quer realmente instalar  o angular material (y)
- Ira perguntar qual tema voce quer instalar.
- Ira perguntar se voce quer o styles do angular material (y)
- Ira perguntar se voce quer adicionar as animações de browser (y)

## Criacao de uma ToolBar com Angular Material
- Primeiro precisamos importar o modulo responsável pela toolbar 
- no site material.angular.io acessar 'Components' > Toolbar
- Em API copiar o código de importação "import {MatToolbarModule} from '@angular/material/toolbar';"
- importar o modulo dentro do arquivo app.module.ts no seu projeto angular, como demostra o print:
  ![image](https://user-images.githubusercontent.com/62728615/140838230-e94317ef-8f7d-4e55-9a0f-14f9985574eb.png)
-Após importado o módulo, adicionar a toolbar do seu gosto copiando o código que existe na aba exemplos dentro da toolbar no site material.angular.io
  ![image](https://user-images.githubusercontent.com/62728615/140838364-37bfdd84-4e62-4e9c-8846-04527cd6f89b.png)
- color="primary" > quer dizer que estará usando a cor primaria do thema escolhido no angular material

##  Criando Modulo e  usando Roteamento com LazyLoading
- Utiliza-se angular CLI para criar o módulo com comando 'ng generate module courses --routing'
- Criação de um component dentro do modulo courses com o comando 'ng generate component courses/courses'
-- Será criado os 4 arquivos que são (html, scss, arquivo de testes spec.ts e o prórpio component )
- Dentro do arquivo de rotas do course (courses-routing-module.ts), adicionar um caminho em branco para direcionar para o CoursesComponent:
  ![image](https://user-images.githubusercontent.com/62728615/140846931-eb6c686e-948e-4791-bfe3-5aad77f8ae21.png)
- Configurar o arquivo de rotas global (app-routing-module.ts), tanto um redirectTo para Course caso tenha apenas localhost:4200 na URL. E um lazyloading para importar o módulo   que usaremos:
  ![image](https://user-images.githubusercontent.com/62728615/140847473-a3b455a3-aab1-4f81-8db0-bd8d20699059.png)
- Dentro do HTML principal <app.component.ts> precisaremos declarar a tag <router-outlet></router-outlet> para o angular entender que estamos usando o roteamento.

## Customizando o tema do Angular material
-  importar '@angular/material/theming'
-  include mat-core();
-  adicionar os 3 tipos de cores existentes no angular material (primary/secondary/warn);
-  criar o tema com as 3 variaveis de cores setadas;
-  alterar o thema padrão do angular material com comando: @include angular-material-theme($custom-theme);
  ![image](https://user-images.githubusercontent.com/62728615/140849770-1b45892e-f598-47c2-bc31-7e1d5a06c78c.png)


