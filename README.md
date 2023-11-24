```console
$ yarn
$ yarn run tsc --build --verbose demos/tsconfig.json
yarn run v1.22.19
warning package.json: No license field
$ /Users/oliver/Code/reduced-test-cases/ts-project-references-augmentation-bug/node_modules/.bin/tsc --build --verbose demos/tsconfig.json
[13:49:06] Projects in this build:
    * app/tsconfig.json
    * demos/tsconfig.json

[13:49:06] Project 'app/tsconfig.json' is out of date because output file 'target/app/tsconfig.tsbuildinfo' does not exist

[13:49:06] Building project '/Users/oliver/Code/reduced-test-cases/ts-project-references-augmentation-bug/app/tsconfig.json'...

[13:49:06] Project 'demos/tsconfig.json' is out of date because output file 'target/demos/index.js' does not exist

[13:49:06] Building project '/Users/oliver/Code/reduced-test-cases/ts-project-references-augmentation-bug/demos/tsconfig.json'...

target/app/index.d.ts:1:63 - error TS2344: Type '"ReadonlyTuple"' does not satisfy the constraint 'keyof URItoKind2<any, any>'.

1 export declare const Apply: import("fp-ts/lib/Apply").Apply2C<"ReadonlyTuple", unknown>;
                                                                ~~~~~~~~~~~~~~~


Found 1 error.
```
