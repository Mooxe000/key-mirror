# KeyMirror

```bash
> before:
'hello'
> after:
{ hello: 'hello' }

-----------

> before:
123
> after:
[Error: keyMirror(...): Argument must be an String or String Array.]

-----------

> before:
null
> after:
[Error: keyMirror(...): Argument must be an String or String Array.]

-----------

> before:
true
> after:
[Error: keyMirror(...): Argument must be an String or String Array.]

-----------

> before:
[ 'hello', 'world' ]
> after:
{ hello: 'hello', world: 'world' }

-----------

> before:
[ 'hello', 123, null ]
> after:
[Error: keyMirror(...): Argument must be an String or String Array.]

-----------

> before:
{ hello: 123, world: false }
> after:
[Error: keyMirror(...): Argument must be an String or String Array.]

-----------
```
