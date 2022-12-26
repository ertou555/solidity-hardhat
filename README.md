# GitVerse

## Step1: install dependencies

 `npm i`

## Step2: add .env

```bash
cp .env.example .env
```

add your private key in the .env file

## Step3: run hardhat node

### 3.1 create hardhat project
```bash
mkdir project
cd project
npm init --yes
npm install --save-dev hardhat
npx hardhat
```
### 3.2 compile contact
```bash
npx hardhat compile
npx hardhat test
```

### 3.3 deploy contact to hardhat localhost network
copy deploy-gitverse.js to hardhat project
```bash
cp deploy-gitverse.js project/scripts/deploy-gitverse.js
```
```bash
npx hardhat --network localhost run scripts/deploy-gitverse.js
or
npx hardhat --network goerli run scripts/deploy-gitverse.js
```

### 3.4 edit gitScript.js
`contractAddress`

### 3.5 edit abi.json

## Step4: tag your repo and run the cmd

```bash
git tag vX.Y.Z
node gitScript.js
```
