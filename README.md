## Sublime Text Snippets for AWS Step Functions

This project defines several snippets that produce JSON code that adheres to the [Amazon States Language specification](https://states-language.net/spec.html)

To start, set the syntax to JSON. These snippets are scoped to JSON syntax files. To begin, type `stepfn + enter`. This will produce the JSON outline and top-level keys:

```
{
	"StartAt": "START_STATE_NAME",
	"Comment": "COMMENT",
	"Version": "VERSION",
	"States": {
		
	}
}
```

The cursor will be placed in the correct position nested under the `"States"` field. To add states, simply begin typing part of the trigger word which corresponds to the state type you wish to use. Hit `tab` to progress forward through the fields and `shift+tab` to move backwards.

The following state types are supported:
| Type 		| Trigger		|
|-----------|---------------|
| Task		| steptask 		|
| Parallel	| stepparallel	|
| Map		| stepmap 		|
| Pass		| steppass		|
| Wait		| stepwait		|
| Choice	| stepchoice	|
| Succeed	| stepsucceed	|
| Fail		| stepfail		|

![Demo](demo.gif)
