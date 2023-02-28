```shell

将NFT文件夹 和metadata文件夹 上传到 https://app.pinata.cloud/


mkdir nft-ipfs
cd nft-ipfs
mkdir hardhat
cd hardhat
npm init --yes
npm install --save-dev hardhat
npx hardhat   -选择Create a Javascript Project

npm install @openzeppelin/contracts
在目录nft-ipfs/hardhat/contracts 下创建 LW3Punks.sol
npm install dotenv

创建.env文件  配置   polygon网络的Mumbai链
QUICKNODE_HTTP_URL="add-quicknode-http-provider-url-here"

PRIVATE_KEY="add-the-private-key-here"

修改scripts/deploy.js
修改 hardhat.config.js
npx hardhat compile
npx hardhat run scripts/deploy.js --network mumbai



-------------
前端
在目录nft-ipfs 下
npx create-next-app@latest
cd my-app
npm run dev
npm install web3modal
npm i ethers@5
修改 Home.modules.css
修改pages/index.js
my-app目录下创建目录constants  并在创建目录下创建文件index.js
配置
export const NFT_CONTRACT_ADDRESS = "address of your NFT contract";
export const abi = "---your abi---";

npm run dev

```
