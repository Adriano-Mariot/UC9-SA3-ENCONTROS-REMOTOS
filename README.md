# Encontros Remotos SA3 UC9 

## Encontro remoto 1 

Atividade desenvolvidas durante o encontro: 
- Instalação do Framework Angular
- Principais funcionalidades 
- Importação do Site E-player

## Encontro remoto 2

Atividades desenvolvidas durante o encontro:
		
		services - interação com apis
		models - modelos de dados da aplicação

Criar um componente
	ng generate component [nome]
	ng generate component components/header 

Site E-PLAYER
	importar o html e o css
	colocar as fontes, css e js na pasta assets
	colocar o arquivo js dentro do angular.json
	instalar o Bootstrap via npm e importar o css e o js do Bootstrap	
	de dentro da pasta dist... para dentro do angular.json (scripts e styles -build)
		

criar um model - ng generate class [nome-da-classe]
	** criar as propriedades email e password dentro do constructor dessa classe - User.ts	
		constructor(
			public email?: string,
			public password?:string
    	){}

	** Criar a variável que instancia/representa o model - dentro de login.component.ts
	** Criar a método/função que receba os dados do form - login.component.ts
		userModel = new User()

		receberDados() {
			console.log(this.userModel);
			
		}


	** Fazer o binding dos campos com o model - login.component.html
		[(ngModel)="userModel.email"] name="email"
		[(ngModel)="userModel.password"] name="password"

	** Implementar o evento de submit no formuário e chamar a função receberDados() - login.component.html
		(ngSubmit)="receberDados()" - dentro do form
	
	** Deixar o botão signin como type-"submit"

