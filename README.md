@@ -1,5 +1,5 @@
#!/bin/bash
set -e

RUSTFLAGS='-C link-arg=-s' cargo +stable build --target wasm32-unknown-unknown --release
RUSTFLAGS='-C link-arg=-s' cargo build --target wasm32-unknown-unknown --release
cp target/wasm32-unknown-unknown/release/whitelist.wasm ./res/
# near
The purpose of this contract is to maintain the whitelist of the staking pool contracts account IDs that are approved by NEAR Foundation.
