## Quick-IC-Vue 1.0.0

A quick Vue template for deployment on the Internet Computer.

This is a create-ic-app template that has been modified. This version runs Vite 2.9.5 and DFX 0.9.2.

### On first clone only:

```
npm install
dfx start --clean --background
dfx deploy
dfx stop
```
Note: These commands generate the core vite files needed to use this program. You only need to do these steps on the first setup. You do not need to have dfx running to use this program unless you have motoko or other on chain functions that depend on a persistent dfx.


### Anytime after initial setup:

Development Server:

```
npm run dev
```

Production Test:

```
npm run serve
```

Generate Dist:

```
npm run build
```
