User: /fix Source "@openzeppelin/contracts/token/ERC20/ERC20.sol" not found: File import callback not supported

VS Code: 1. Use the Terminal: Create New Integrated Terminal command.
2. In the terminal, run `npm install @openzeppelin/contracts` in your workspace root so the `@openzeppelin/contracts` import resolves.
3. If your Solidity file is inside a subfolder and your project root is above it, enable `solidity.monoRepoSupport`.



Show in Settings Editor

User: 按照D:\www6.5sy\WWW6.5\Shaoyan的内容，编写一份readme文档

Workspace: Collecting workspace information# Web3 Solidity Contracts 集合

这是 Shaoyan 目录下的 Solidity 合约集合，包含从基础合约到中级 DeFi、DAO、NFT、市集等多个示例项目。

## 项目结构

- package.json
- day1_clickcounter.sol
- day2_savemyname.sol
- day3_candidatename.sol
- day4_auctionhouse.sol
- day5_adminonly.sol
- day6_etherpiggybank.sol
- day7_simpleIOU.sol
- day8_tipjar.sol
- day9_1ScientificCalculator.sol
- day9_2Calculator.sol
- day10_ActivityTracker.sol
- day11_1Ownable.sol
- day11_2VaultMaster.sol
- day12_SimpleERC20.sol
- day13_1MyToken.sol
- day13_2Preordertoken.sol
- day14_MultisigDepositBox.sol
- day15_GasEfficientVoting.sol
- day16_1PluginStore.sol
- day16_2AchievemenPplugin.sol
- day16_3WeaponStorPlugin.sol
- day17_1Subscriptionstorage.sol
- day17_2SubscriptionLogicV1.sol
- day17_3SubscriptionLogicV2.sol
- day18_1MockWeatherOracle.sol
- day18_2CropInsurance.sol
- day19_SignThis.sol
- day20_1GoldVault.sol
- day20_2GoldThief.sol
- day21_SimpleNFT.sol
- day22_DecentralisedLottery.sol
- day23_LendingPool.sol
- day24_DecentraliseEscrow.sol
- day25_AMM.sol
- day26_NFTMarketplace.sol
- day27_YieldFarming.sol
- day28_1GovernanceToken.sol
- day28_2DAOGovernance.sol
- day29_1StableCoin.sol
- day30_1MockToken.sol
- day30_3MiniDexFactory.sol

## 合约概要

- day1_clickcounter.sol
  - 简单计数器合约

- day2_savemyname.sol
  - 存储个人信息、名称、简介、年龄和职业枚举

- day3_candidatename.sol
  - 候选人名称管理与投票计数

- day4_auctionhouse.sol
  - 英式拍卖实现，包含事件、竞拍、结束拍卖、赢家查询

- day5_adminonly.sol
  - 管理员授权提款系统，包含提取额度与拥有者控制

- day6_etherpiggybank.sol
  - 会员存款与提款，模拟储蓄金库

- day7_simpleIOU.sol
  - 朋友注册、钱包存款、债务记录与偿还

- day8_tipjar.sol
  - 小费罐，支持多货币兑换、ETH 小费、提现与所有权转移

- day9_1ScientificCalculator.sol
  - 科学计算器：幂运算与整数平方根

- day9_2Calculator.sol
  - 调用外部科学计算器合约，演示高级调用与低级调用

- day10_ActivityTracker.sol
  - 用户运动记录、历史、里程碑事件

- day11_1Ownable.sol
  - 基础 `Ownable` 合约

- day11_2VaultMaster.sol
  - 继承 `Ownable` 实现可提取金库

- day12_SimpleERC20.sol
  - 简化 ERC20 代币实现

- day13_1MyToken.sol
  - 自定义代币合约

- day13_2Preordertoken.sol
  - 预售代币，包含锁定转账与售卖逻辑

- day14_MultisigDepositBox.sol
  - 多签秘密存储与读取审批

- day15_GasEfficientVoting.sol
  - 气体优化投票，使用位运算压缩投票记录

- day16_1PluginStore.sol
  - 插件存储与动态调用系统

- day16_2AchievemenPplugin.sol
  - 成就插件

- day16_3WeaponStorPlugin.sol
  - 武器装备插件

- day17_1Subscriptionstorage.sol
- day17_2SubscriptionLogicV1.sol
- day17_3SubscriptionLogicV2.sol
  - 订阅存储布局与逻辑扩展，包含暂停/恢复与订阅查询

- day18_1MockWeatherOracle.sol
  - 模拟天气预言机

- day18_2CropInsurance.sol
  - 农作物保险，基于天气预言机赔付

- day19_SignThis.sol
  - 签名签到系统，演示 ECDSA 签名验证与批量签到

- day20_1GoldVault.sol
  - 金库，包含安全取款与漏洞示例

- day20_2GoldThief.sol
- day21_SimpleNFT.sol
  - 重入攻击合约示例，针对 `GoldVault` 漏洞

- day22_DecentralisedLottery.sol
  - 去中心化彩票，生成随机赢家并支付奖金

- day23_LendingPool.sol
  - 借贷池，支持存款、抵押、借款、还款与利息计提

- day24_DecentraliseEscrow.sol
  - 去中心化托管，支持交付确认、争议与超时退款

- day25_AMM.sol
  - 简易自动做市商，实现流动性添加与代币交换

- day26_NFTMarketplace.sol
  - NFT 市场：上架、取消上架、购买、转账和退款

- day27_YieldFarming.sol
  - 质押挖矿合约，支持质押、奖励、紧急取回和补充奖励

- day28_1GovernanceToken.sol
- day28_2DAOGovernance.sol
  - DAO 治理代币与治理合约，包含提案、投票、治理仓库、时锁与押金

- day29_1StableCoin.sol
  - 简单稳定币引擎，支持 mint、burn 与转账

- day30_1MockToken.sol
- day30_3MiniDexFactory.sol
  - 模拟 ERC20 代币与迷你 Dex 工厂合约

## 依赖说明

- package.json
  - 依赖：`@openzeppelin/contracts`
  - 当前没有定义测试脚本

## 使用说明

1. 安装依赖
```sh
npm install
```

2. 如果使用 Hardhat、Foundry 或 Remix，请将 Shaoyan 目录作为 Solidity 源文件路径加载

3. 合约文件均为独立示例，可分别编译与部署

## 备注

- 本仓库主要用于学习 Solidity 合约设计与模式
- 部分合约用于演示安全漏洞与防护
- 如果需要进一步编译/测试，可在项目根目录补充 Hardhat 或 Foundry 配置文件
