# ePOW, Eclipse $BITZ Setup Guide on Ubuntu 💚


1. Install Rust
```bash 
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
2. Follow the prompts. Once installed, run:
```bash
source $HOME/.cargo/env
```
3. Install Solana CLI
```bash 
curl --proto '=https' --tlsv1.2 -sSfL https://solana-install.solana.workers.dev | bash
```
4. Create a Wallet (Keypair)
```bash
solana-keygen new
```
Set Passphrase for better security or just skip (click enter)

This will create a new keypair at the default path: ```~/.config/solana/id.json```

Save your public key & mnemonic — it will be shown after creation.
<br><br>
<br><br>
5. Install Bitz CLI
```bash
cargo install bitz
```
6. Change RPC
```bash
solana config set --url https://mainnetbeta-rpc.eclipse.xyz/
```
  or
```bash
solana config set --url https://eclipse.helius-rpc.com/
```
7. Open Screen
```bash
screen -S eclipse
```
8. Start eMining
```bash
bitz collect
```
You need 0.005 $ETH on Eclipse to start mining, so send $ETH to your public key
<br><br>
Other Commands:

  •	Claim your Bitz:
```bitz claim```
  
  •	Check your balance:
```bitz account```

  • Config CPU (change the number to change cores):
```bitz collect --cores 8```
  
  •	View all commands:
```bitz -h```
<br><br>
Import to backpack:
```bash
solana config get
```
copy path of Keypair path 
```bash
cat <Keypair path>
```
Copy array of number and import them on backpack in private key section
<br><br>
<br><br>
**For help check #powpow channel on Eclipse discord: https://discord.gg/eclipse-fnd**
<br><br>
**My X: https://x.com/ArshiaXBT**
