### Title :What Happens to TypeScript During Compilation (tsc) \& The Role of tsconfig.json





#### ***Introduction:***



TypeScript is a superset of JavaScript that adds static typing to JavaScript. Browsers and Node.js cannot directly execute TypeScript code in the traditional workflow. Therefore, TypeScript code must be compiled into JavaScript using the TypeScript compiler (tsc). During compilation, TypeScript checks for type-related errors and transforms the code into JavaScript.



###### **Happening During TypeScript Compilation:**



* **Reading TypeScript Files:**

&#x09;The compiler reads .ts files and analyzes their structure, variables, functions, 	interfaces, and types.



* **Type Checking**

&#x09;The compiler checks whether variables, function parameters, and return values 		follow their declared types.



* **Transpiration**

&#x09;TypeScript removes type annotations and converts TypeScript syntax into 	JavaScript.



* **JavaScript Output**

&#x09;The compiler generates .js files based on the configured target. These JavaScript 	files can then run in browsers or Node.js.



#### **Role of tsconfig.json:**



tsconfig.json is the configuration file for a TypeScript project. It controls how the TypeScript compiler checks and compiles files.



#### **Example:**

&#x09;{

&#x20; "compilerOptions": {

&#x20;   // File Layout

&#x20;   "rootDir": "./src",

&#x20;   "outDir": "./dist",

&#x20;   "module": "esnext",

&#x20;   "target": "esnext",

&#x20;   "strict": true,

&#x20;   "moduleDetection": "force",

&#x20;   "skipLibCheck": true

&#x20; }

}



* target: Specifies the JavaScript version.
* rootDir: Specifies the source directory.
* outDir: Specifies the output directory.
* module: Defines the module system.
* strict: Enables strict type checking.



#### ***Conclusion:***



tsc checks TypeScript code, reports type errors, and generates JavaScript files. Meanwhile, tsconfig.json controls the compiler's behavior through configurable options, making TypeScript projects easier to manage and maintain.

