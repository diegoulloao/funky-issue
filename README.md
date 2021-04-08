# Funk issue
Repository provided in order to fix the https://github.com/RobertBroersma/funk/issues/1 bug.

## Information
This is a Next js web application. The issue is happening when changing between pages.

## Start the development server

First, run the command:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Gitpod
You can open the repository directly in Gitpod

<a href="http://gitpod.io/#https://github.com/diegoulloao/funky-issue" target="_blank">
  <img src="https://gitpod.io/button/open-in-gitpod.svg" alt="">
</a>

## How to reproduce the issue
1. Go to initial page
2. Press link "Go to another page"

The following error should appear:
```
Unhandled Runtime Error
TypeError: Cannot read property 'removeEventListener' of null
```

Extended log:
```
Unhandled Runtime Error
TypeError: Cannot read property 'removeEventListener' of null

Call Stack
eval
webpack-internal:///./node_modules/@statikly/funk/dist/funk.esm.js (222:33)
HTMLUnknownElement.callCallback
webpack-internal:///./node_modules/react-dom/cjs/react-dom.development.js (3945:14)
Object.invokeGuardedCallbackDev
webpack-internal:///./node_modules/react-dom/cjs/react-dom.development.js (3994:16)
invokeGuardedCallback
webpack-internal:///./node_modules/react-dom/cjs/react-dom.development.js (4056:31)
flushPassiveEffectsImpl
webpack-internal:///./node_modules/react-dom/cjs/react-dom.development.js (23538:11)
unstable_runWithPriority
webpack-internal:///./node_modules/scheduler/cjs/scheduler.development.js (468:12)
runWithPriority$1
webpack-internal:///./node_modules/react-dom/cjs/react-dom.development.js (11276:10)
flushPassiveEffects
webpack-internal:///./node_modules/react-dom/cjs/react-dom.development.js (23442:14)
eval
webpack-internal:///./node_modules/react-dom/cjs/react-dom.development.js (23319:11)
workLoop
webpack-internal:///./node_modules/scheduler/cjs/scheduler.development.js (417:34)
flushWork
webpack-internal:///./node_modules/scheduler/cjs/scheduler.development.js (390:14)
MessagePort.performWorkUntilDeadline
webpack-internal:///./node_modules/scheduler/cjs/scheduler.development.js (157:27)
```
