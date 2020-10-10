# pokedex-app
A Builiding an App from scratch using Typescript HTML CSS


## Setup Typescript
`yarn add -g typescript`
`or`
`npm install -g typescript`

## Configuring TypeScript with tsconfig
tsconfig is a JSON file that helps to configure TypeScript. Having a config file is better since it helps to control the behavior of the compiler. 

`tsc init`

## tsconfig file
```
{
    "compilerOptions": {
        "target": "es5",
        "module": "commonjs",
        "outDir": "public/js"
        "rootDir": "src",
        "strict": true,
        "esModuleInterop": true
        "forceConsistentCasingInFileNames": true
    },
    "include": ["src"]
}
```

This config file is much verbose than that, I removed the comments and unused values to make it easy to read.

## Compile Typescript to Javascript

`tsc`


This command will compile every file with .ts extension to JavaScript. And since we have a tsconfig file, the compiler will follow the defined rules and compile only the TS files located in the src folder and put the JS code into the public directory.

If you want not to execute the commend on every change, just add a `-w` flag to let compiler to keep watching for a change and re-compile when necessary.

`tsc -w`


Inspired from https://github.com/ibrahima92/pokedex-typescript
