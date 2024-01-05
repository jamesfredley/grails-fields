
- `master` new coordinate: `io.github.gpc:fields:4.0.0-RC1` - Grails 4.x 
- `3.0.0.RC1` last version on coordinates: `org.grails.plugins:fields:3.0.0.RC` - Grails 4.x 
- `2.2.x` y `2.1.x` for Grails 3. 
- `grails2.x` for Grails 2.

A spiritual successor to the bean-fields plugin that attempts to provide a configurable way to render forms with appropriate inputs for different properties without having to copy and paste lots of boilerplate code. It should be possible to change the rendering for a field with the minimum of impact on any other code. This plugin attempts to achieve that by using GSP templates looked up by convention. Developers can then create templates for rendering particular properties or types of properties with the former overriding the latter.

For further information please see the full documentation.

Documentation can be found [here](https://gpc.github.io/fields)

## Important 

If you use `org.grails.plugins:scaffolding` version 4.10.0 or less you need to exclude the original `org.grals.plugins:fields:3.3.0.RC1` like this:

```
implementation("org.grails.plugins:scaffolding") {
  exclude module: 'fields'
}
implementation 'io.github.gpc:fields:5.0.0-RC2'
```

if you are using Grails 4.x, replace `implementation` with `compile` and use `io.github.gpc:fields:4.0.0`. 

GA versions for Grails 5.x and 6.x are pending
