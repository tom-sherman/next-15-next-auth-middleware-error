## Steps to reproduce

1. `pnpm i`
2. `pnpm dev`
3. Load localhost:3000, returns ok
4. Stop dev server and rm -rf .next to make sure no caches
5. `pnpm dev-turbo

## Expected behavior

Should be able to load localhost:3000

## Actual behaviour

```
⨯ Error [TypeError]: _react.default.createContext is not a function
    at Object.<anonymous> (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/_cafd18._.js:11709:41)
    at [project]/node_modules/.pnpm/next@15.0.0-canary.25_react-dom@19.0.0-rc-6f23540c7d-20240528_react@19.0.0-rc-6f23540c7d-2024_b7zrpq6fnlnpp5u2olazipblr4/node_modules/next/dist/shared/lib/app-router-context.shared-runtime.js [middleware] (ecmascript) (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/_cafd18._.js:11721:3)
    at <unknown> (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:555:27)
    at runModuleExecutionHooks (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:597:9)
    at instantiateModule (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:553:9)
    at getOrInstantiateModuleFromParent (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:625:12)
    at commonJsRequire (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:156:20)
    at Object.<anonymous> (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/_cafd18._.js:12380:40)
    at [project]/node_modules/.pnpm/next@15.0.0-canary.25_react-dom@19.0.0-rc-6f23540c7d-20240528_react@19.0.0-rc-6f23540c7d-2024_b7zrpq6fnlnpp5u2olazipblr4/node_modules/next/dist/client/components/navigation.js [middleware] (ecmascript) (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/_cafd18._.js:12472:3)
    at <unknown> (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:555:27)
 ⨯ Error [TypeError]: _react.default.createContext is not a function
    at Object.<anonymous> (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/_cafd18._.js:11709:41)
    at [project]/node_modules/.pnpm/next@15.0.0-canary.25_react-dom@19.0.0-rc-6f23540c7d-20240528_react@19.0.0-rc-6f23540c7d-2024_b7zrpq6fnlnpp5u2olazipblr4/node_modules/next/dist/shared/lib/app-router-context.shared-runtime.js [middleware] (ecmascript) (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/_cafd18._.js:11721:3)
    at <unknown> (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:555:27)
    at runModuleExecutionHooks (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:597:9)
    at instantiateModule (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:553:9)
    at getOrInstantiateModuleFromParent (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:625:12)
    at commonJsRequire (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:156:20)
    at Object.<anonymous> (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/_cafd18._.js:12380:40)
    at [project]/node_modules/.pnpm/next@15.0.0-canary.25_react-dom@19.0.0-rc-6f23540c7d-20240528_react@19.0.0-rc-6f23540c7d-2024_b7zrpq6fnlnpp5u2olazipblr4/node_modules/next/dist/client/components/navigation.js [middleware] (ecmascript) (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/_cafd18._.js:12472:3)
    at <unknown> (file:///home/tom/code/next-15-next-auth-middleware-error/.next/server/edge/chunks/ssr/edge-wrapper_5f3c4e.js:555:27)
```
