1. deno --version

```
deno 1.5.2 (71d7482, release, x86_64-apple-darwin)
v8 8.7.220.3
typescript 4.0.5
```

`export default function myFunction()` would be the only entry point for frist_bundle module"

2. deno bundle first_bundle/main.js first_bundle.js

bundle the bundle:

3.  deno bundle main.js final_result.js

final_result.js contains this:

```
function square(a) {
    return a * a;
}
console.log(entry());
```

instead of calling entry() it should be referencing exported default function from first bundle