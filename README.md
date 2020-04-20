# Angular Development Information

## Setup
* *nix
  * Software Dependencies:
    * nodejs
  * Framework
    * Automated Test - use either one of the following
      * <b>Jest</b>
        * URL : https://jestjs.io/
        * Installation
          * npm install <b>jest</b> @types/jest --only=dev
          * npm install jest-preset-angular
          * Add <b>jest</b> configuration to <b>package.json</b>
          * ```json 
                {
               "name": "my-package",
               "version": "0.0.1",
               "license": "MIT",
               "scripts": {
                "test": "jest",
                "test:watch": "jest --watch",
                "test:cc": "jest --coverage"
               },
               "dependencies": {
                "@angular/common": "7.2.1",
                "@angular/compiler": "7.2.1",
                ...
               },
               "devDependencies": {
                "@types/jest": "^25.2.1",
                "jest": "^25.4.0",
                "jest-preset-angular": "^8.1.3",
                ...
               },
               "jest": {
                "preset": "jest-preset-angular",
                "setupTestFrameworkScriptFile": "<rootDir>/setupJest.ts"
               }
              }
            ```
          * Sample <b>setupJest.ts</b>
              ```
                import 'jest-preset-angular';
              ```
          * Remove jasmine 
              * npm uninstall jasmine @types/jasmine 
      * Jasmin & Karma
* Windows 10
