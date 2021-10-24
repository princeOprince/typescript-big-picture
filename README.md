# TypeScript - The Big Picture

This is a summary of the pluralsight course [TypeScript: The Big Picture][1]

***

### Benefits
+ Typescript supports static typing
+ Typescript supports type inference
+ Typescript provides parameter and automatic function invocation checking
+ Typescript helps with code organisation - classes, namespaces, 
  modules, interfaces
+ Typescript provides tooling support - static type analysis,
  code completion, detect unused data and unreachable code,
  generate source maps (debug in typescript)
+ Typescript provides type annotation - information about a variable
  when you mouse over it (in VSCode)
  
***

### Installing and Compiling
+ The Typescript compiler is `tsc`
+ A typescript file has the extension `.ts`
+ Typescript transpiles (translate + compile) to Javascript
+ Install Typescript globally with `npm`

```TypeScript
npm install -g typescript
tsc -v  // check version
tsc -h  // help
```

***

### Compiler options
+ `target` - specify ECMAScript version
+ `outDir` - location of the output file
+ `outFile` - name of the output file
+ `lib` - library files to be loaded
+ `watch` - automatic check for code changes

```TypeScript
tsc --target es2015 --outDir js script.js
```

***

### Configuration
+ `tsc` checks for a `tsconfig.json` config file when run
+ `tsc` uses default settings if config file not found
  + compiles to `es3`
  + stores transpiled `.js` file in the same location as `.ts` file
  

```TypeScript
tsc --init    // generate an editable config file
tsc           // run tsc to compile without providing filename
```

***

### Use case
+ Typescript is a superset of Javascript
+ All Javascript code is valid in Typescript
+ Use colon to explicitly specify variable types, return types
  and parameter types

```TypeScript
const age : int = 10;
function myfunction(name: string, age: int) : void {}
```

***

![big-picture-certification](typescript1.png)


[1]: https://www.pluralsight.com/courses/typescript-big-picture
