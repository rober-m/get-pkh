# get-pkh

Website to get your wallet's PKH 

## Steps:

0. Clone this repository and `cd` into it
1. Go to [Blockfrost.io](blockfrost.io) to get your own ProjectID (the network is irrelevant)
2. Replace your ProjectID in the `index.html` file as shown:
```js
            new Blockfrost("https://cardano-preview.blockfrost.io/api/v0", "<ProjectID>"),
            // to
            new Blockfrost("https://cardano-preview.blockfrost.io/api/v0", "preview0123abc456def"),
            
```
3. Run `node app.js`
4. Open [localhost:3000](http://localhost:3000)
5. Make sure to have a Nami wallet with the wallet you want to complete the challenge. If you prefer to use a different wallet, change the code to reflect that (e.g., if you want to use Lace, change line 15 to `const api = await window.cardano.lace.enable()`)
6. Click "Get PKH" button.
7. Submit the PKH printed below to IOG's form.