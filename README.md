# angular_2_curso
1-começar projeto
    ng new nomeprojeto --strict 
        strict habila varias verificaçoes
2-prettier
    npm install --save-dev prettier
    npm install --save-dev tslint-config-prettier
    npm install --save-dev tslint-plugin-prettier
    "extends": ["tslint:recommended", "tslint-plugin-prettier", "tslint-config-prettier"]
3- instalar bootstrap   
    npm i bootstrap font-awesome
    Para que todos os componentes do projeto peguem o componente do bootstrap tem que ir no arquivo
    angular.json   > styles
        "./node_modules/bootstrap/dist/css/bootstrap.min.css",
        "./node_modules/font-awesome/css/font-awesome.css"

4-Criacao de modulo
    ng genetae module  NOMEMODULO --routing -d
        routing já cria a rota
        d executa dryRun:ou seja não cria as pastas mas mostra onde esta criando como simulçao
    quando se trabalha com mosulo deve-se exportar ele. Criando a tag export e importando ele no app.module
5-criar rota-Lease loud
    router-outlet

6-formulario template
    import FormsModule

7-passar dados entre componentes
    Adiciona o decorator @input() Nome variavel no ts que vai receber
    No mudolu cria a o export do commponent
    No modulo que vai passar a ainformação faz um iport com o modulo que vai passar a ainformaão
    Quando fizer isso dentro da chamada do componente pode se adicionar o atributo e o valor criado
8- #campoUsuario="ngModel" no html permite pegar os estados do input e armazenar na vairiavel com a #
9-ao se colocar colchetes [] em uma propriedade do html, ela vai permitr fazer uma logica de
10-para verificar os dadso passadados no login
    Abre o conseole do navegador >> Rede >> opcao XRH >>Seleciona a pagina que fez a requisicao
    Proucra o X-access-COntent >> copia ele e joga no site jwt e ve as infroamçoes
    Para usar no projeto Intalar bibiloteca npm i jwt-decode