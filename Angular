***ANGULAR***

**CLI**

criação do projeto - ng new "nome do projeto angular"
criação do component - ng g c 'nome do componente' 
criação de modulo - ng g m 'nome do modulo'
gerar componente dentro de um modulo - ng g c "module/componente"
servidor local - ng serve

**DIRETIVAS**  - é um comando especial do angular para chamar efeitos/comportamentos de script de maneira mais facil

[ngIf] - condicional (ex: [ngIf]="false")
[ngFor] - laço de repetição (ex: <li *ngFor="let elemento of lista">{{elemento}} </li>)
[ngClass] - atribuição de classe (ex: <p [ngClass]="estilo">comp-atributos works!</p>)
[ngStyle] - att de estilo (ex: <h1 [ngStyle]="{'background': corFundo, 'color': corFonte}">CURSO ANGULAR</h1>)
[ngSwitchCase] - condicional (ex:
	<div [ngSwitch]="menuType">
	  <div *ngSwitchDefault>
	    <ul>
	      <li> editar perfil </li>
	      <li> adicionar cartão </li>
	    </ul>
	  </div>
	  <div *ngSwitchCase="'admin'">
	    <ul>
	      <li> editar perfil </li>
	      <li> adicionar cartão </li>
	      <li> gerenciar usuarios</li>
	    </ul>
	  </div>
	  <div *ngSwitchCase="'superuser'">
	    <ul>
	      <li> editar perfil </li>
	      <li> adicionar cartão </li>
	      <li> gerenciar usuarios</li>
	      <li> gerenciar admins </li>
	    </ul>
	  </div>
	</div>
)

[(ngModel)] - iteração html com ts (ex:
	<input type="text" [(ngModel)]="item">
	<button (click)="adicionarLista()">add</button>
	<p>{{item}}</p>
)

<ng-content select='tagHtml'></ng-content select> - TAG QUE BUSCA DO PAI
<ng-template> - TAG QUE FICA OCULTA E SÓ APARECE COM UMA CONDICIONAL	(ex:
	<ng-template [ngIf]="false">
	<a href="#">adicionar ao carrinho</a>
	</ng-template>
)








