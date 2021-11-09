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
