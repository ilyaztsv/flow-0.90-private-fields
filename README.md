# flow-0.90-private-fields

The repo for [flow/issues/7355](https://github.com/facebook/flow/issues/7355).

```bash
npm i

npm run typecheck
```

Output:

```bash
Error ┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈ src/index.js:0:1

Unexpected parser state: "Assert_failure src/parser_utils/signature_builder_generate.ml:653:58"



Found 1 error
npm ERR! code ELIFECYCLE
npm ERR! errno 2
npm ERR! flow-0.90-private-fields@1.0.0 typecheck: `flow`
npm ERR! Exit status 2
npm ERR!
npm ERR! Failed at the flow-0.90-private-fields@1.0.0 typecheck script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.
```

But if you'll do the following:

```bash
npm i flow-bin@0.89.0

npm run typecheck
```

Output:

```bash
No errors!
```