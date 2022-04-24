## Quick IC Vue 1.1.0

A quick Vue template for deployment on the Internet Computer.

This is a Vue/TypeScript template that was generated using create-ic-app and then modified to fit specific use cases of the CP team. Comes with custom boilerplate code in default dark mode and is configured for DFX 0.9.2.
<br>
<br>

### On first clone only:

```
npm install
dfx start --clean --background
dfx deploy
dfx stop
```
Note: These commands generate the core vite files needed to use this program. You only need to do these steps on the first setup. You do not need to have dfx running to use this program unless you have motoko or other on chain functions that depend on a persistent dfx.
<br>
<br>
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
