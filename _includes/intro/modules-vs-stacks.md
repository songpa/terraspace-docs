## Modules vs Stacks

Both modules and stacks are terraform modules. The difference is organizational and how they are meant to be used.

* Modules are reusable pieces of code. Generally, it contains non-business specific logic.
* Stacks are meant to be used to group together modules. Generally, this is where business-specific logic goes.

For example, the `app1` stack could be designed to use the `instance` module. Another, `app2` stack could use the `instance` and `rds` modules.
