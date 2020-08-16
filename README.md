# knockout-subsequent-variable-declarations
## Steps
1. Run `yarn`
2. Run `yarn typecheck`
```
Done in 2.83s.
```
3. Uncomment the second line in `index.ts`
4. Run `yarn typecheck`
```
node_modules/@types/knockout/index.d.ts:1062:13 - error TS2403: Subsequent variable declarations must have the same type.  Variable 'ko' must be of type 'typeof import("d:/Projects/knockout-subsequent-variable
-declarations/node_modules/knockout/build/types/knockout")', but here has type 'KnockoutStatic'.

1062 declare var ko: KnockoutStatic;
                 ~~

  node_modules/knockout/build/types/knockout.d.ts:5:1
    5 export as namespace ko;
      ~~~~~~
    'ko' was also declared here.


Found 1 error.

error Command failed with exit code 1.
```
