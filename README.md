# angularNotes
Simple notes for me to reference, using my own language and thoughts. 

Angular Notes 

@Input() 
This requires 3 things
	- Parent component must pass variable to child component (ex. <my-component [name]=variable></my-component>).
	- Child component must import { Input } from '@angular/core';
	- Child component must @Input() displayText; 

<ng-content></ng-content>
Using ng-content allows you to put a hook that you 
can put custom html into your component. Without putting
ng-content within your custom component, angular will remove 
it from the DOM.

Service Requirements
	-Service Created via a .ts file with a export class
		-export class ServiceClassName(){
			functions...
		}
	-In component
		-Import { ServiceClassName} from './path'
		-providers: [ServiceClassName]
		-public serviceVariableName: ServiceClassName in constructor
