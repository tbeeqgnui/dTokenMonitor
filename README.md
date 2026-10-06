# dToken Monitor

Static dashboard for monitoring dToken fund allocation and manually preparing rebalance transactions on Ethereum and BSC.

## Run locally

```bash
./start-server.sh
```

Open `http://localhost:8000`.

## Deploy

Import this repository into Vercel. The app is plain HTML, CSS, and JavaScript, so no build command or output directory is required.

## Notes

- Public RPC endpoints are configured on the asset buttons in `index.html`.
- Rebalance simulation uses `eth_call` and `estimateGas` before a wallet sends a transaction.
- Production RPC credentials must not be committed or exposed in browser code.

