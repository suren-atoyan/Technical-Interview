Status - In progress.

## JavaScript programming language questionnaires as an interview guide.

### JavaScript and Ecosystem

* Please introduce JavaScript as a programming language in a few sentences with your words as it is convenient for you.
  * Interpreted or compiled language.
    * The above explanation.
    * Advantages/Disadvantages.
    * The differences compared with other languages.
    * JIT (Jast In Time ) compiler.
  * Dynamically or statically typed.
    * The above explanation.
    * The difference compared with other languages.
    * Advantages/Disadvantages.
    * Impact on performance.
  * What is multi-paradigm?
  * Works as a single threaded / multi threaded.
    * The above explanation.
    * Examples.
    * The differences compared with other languages.
    * Advantages/Disadvantages.
  * Try to define "Fundamentals of Functional programming".
    * JavaScript as a Functional Programming Language.
* Functions by declaration type.
  * Function declaration / expression function.
    * The difference.
  * Lexical Environment / Variable Environment.
* Hoisting.
* ES6, ES7, ES8
  * Block Scope
    * For variables
      * Let / Const
        * Compare with "var"
        * Are they hoisted?
    * For functions
  * Arrow Functions
    * Compare with es5 functions
  * Template Literals
  * Destructuring assignment
    * Array destructuring
    * Object destructuring
    * Deep matching - Nested destructuring
    * The Rest operator
    * Function parameters
    * Default values
  * Object Properties
    * Shorthand names
    * Computed names
  * Modules
    * ES6 modules
      * import
      * export
      * export … from …
    * Async import (es8)
      * import(...)
    * importScripts(...) - Web Workers
    * World "before" es6 modules
      * AMD - asynchronous module definition
        * RequireJS
          * Realization by 50 LOC
        * UMD
        * CommonJs
    * Classes
        * Class declaration
        * Class expression
        * Static methods
        * Getter / setter
        * Class inheritance
    * Promises
        * Promises/A+
        * Realization in es5
        * Async / await
    * Generators
        * Function generator
        * Async generators
    * Symbol type
    * Iterators
    * Proxy
    * Reflect
    * Typed Arrays
      * Int8Array()
      * Uint8Array()
      * Uint32Array()
      * Float32Array()
      * Uint8ClampedArray()
      * Int16Array()
      * Uint16Array()
      * Int32Array()
    * SIMD (low-level data parallelism)
    * Shared memory and atomics
* Which features from es6,7,8 are have a fully or partially compatibility with es5?
  * Examples.
    * Classes
    * Generators
    * Promises
    * Modules
    * and etc.
* Web APIs
  * Web workers
    * Dedicated workers
    * Service workers
    * Shared workers
    * Audio workers ( Worklet )
  * windowTimers
    * setTimeout / setInterval / setImmediate
      * Describe setTimeout as a function.<br/>* Not important questions: <br/>1. Can the first argument of setTimeout not be a function? <br/>2. Is there a third argument for setTimeout, if yes what does it represent and has it limitations, if yes, then what kind of limitations?
      * Give a mathematical claim for the second argument of setTimeout.
      * Detailed description of setTimeout's work.
      * Recursive setTimeout and setInterval.
      * setTimeout (fn, 0) as an exception.
      * Dom minimum timeout value.
      * setImmediate, setImmediate 's polyfill, polyfill implementation.<br /> * postMessage <br /> * messageChannel <br /> * <script> onreadystatechange.
      * process.nextTick, Promise.resolve(). Compare with setTimeout().
      * Task, MicroTask, differences, execution order, implementation in different browsers.
      * setTimeouts’ execution order - FIFO, LIFO, random.
  * Client side storages.
    * IndexedDB
    * WebSql
    * localStorage
    * Session storage
  * Categories of Web APIs
    * Communication APIs
    * Data management APIs
    * Hardware access APIs
    * Other APIs
* Tools/libraries/frameworks from ecosystem of JavaScript
  * Task runners, builders, source-to-source compilers, optimization tools.
    * Gulp
    * Grunt
    * Webpack
    * Prepack
    * UglifyJs
    * Babel
  * Libraries/Frameworks
    * What kind of problems do they wanted to solve, when they created this very tool?
    * For example, when we talk about ReactJs, what problems does it solve, what kind of approaches have other tools for solving such problems? For example tools like:
      * BackboneJS
	    * KnockoutJS
	    * jQuery
    * React
  * Angular
  * Polymer
  * Vue
* Engine
  * Parsing
    * Lazy Parsing
      * Pre parsing
      * Full parsing
  * Tockenazing/Lexing
  * AST ( Abstract Syntax Tree )
  * JIT (Just in Time compiler)
    * Compile + Optimization
    * Re-optimization / De-optimization
  * Automate Memory Management - GC
    * Comparison with manual memory management
    * advantages / disadvantages
* Web Assemble
  * toolchain
    * emscripten
    * clang
    * llvm
  * Detailed description of webassembly work.
  * etc.

#### Discussion of Situations.

...

#### Related topics.

* NodeJs
* Networking
	* TCP/IP
	* HTTP
		* HTTP 0.9 - 1.1
		* HTTP/2
	* HTTPS
	* HSTS
	* WebSocket
* Web Servers
	* Nginx
	* Apache
* AMQP
	* RabbitMQ
	* ZeroMQ
* DBs
	* Relational Databases
		* MySQL
		* MariaDB
		* PostgreSQL
	* NoSQL
		* MongoDB
			* Minimongo - as a client side db wrapper
		* CouchDB
			* PouchDB - as a client side db wrapper
    * Redis

#### Disclaimer

This document is still draft and needs to be improved.

    
