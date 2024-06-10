# Hyperlane Warp Route Gas Report

Run test from https://github.com/hyperlane-xyz/hyperlane-monorepo/blob/main/solidity/test/token/HypERC20.t.sol

## Gas Report

Compiling 286 files with 0.8.22
Solc 0.8.22 finished in 25.95s
Compiler run successful!

Ran 4 tests for test/token/HypERC20.t.sol:HypFiatTokenTest
[PASS] testBenchmark_overheadGasUsage() (gas: 77344)
Logs:
  Overhead gas usage: 68915

[PASS] testHandle() (gas: 93462)
[PASS] testRemoteTransfer() (gas: 338862)
[PASS] testTransfer_withHookSpecified() (gas: 273832)
Suite result: ok. 4 passed; 0 failed; 0 skipped; finished in 9.83ms (2.51ms CPU time)

Ran 6 tests for test/token/HypERC20.t.sol:HypERC20CollateralTest
[PASS] testBenchmark_overheadGasUsage() (gas: 78408)
Logs:
  Overhead gas usage: 70023

[PASS] testInitialize_revert_ifAlreadyInitialized() (gas: 187)
[PASS] testRemoteTransfer() (gas: 335522)  
[PASS] testRemoteTransfer_invalidAllowance() (gas: 145332)
[PASS] testRemoteTransfer_withCustomGasConfig() (gas: 460606)
[PASS] testTransfer_withHookSpecified() (gas: 271481)
Suite result: ok. 6 passed; 0 failed; 0 skipped; finished in 9.79ms (3.30ms CPU time)

Ran 6 tests for test/token/HypERC20.t.sol:HypNativeTest
[PASS] testBenchmark_overheadGasUsage() (gas: 76874)
Logs:
  Overhead gas usage: 68489

[PASS] testInitialize_revert_ifAlreadyInitialized() (gas: 165)
[PASS] testRemoteTransfer() (gas: 223265)
[PASS] testRemoteTransfer_invalidAmount() (gas: 140302)
[PASS] testRemoteTransfer_withCustomGasConfig() (gas: 341768)
[PASS] testTransfer_withHookSpecified() (gas: 257067)
Suite result: ok. 6 passed; 0 failed; 0 skipped; finished in 9.94ms (2.92ms CPU time)

Ran 5 tests for test/token/HypERC20.t.sol:HypXERC20LockboxTest
[PASS] testApproval() (gas: 24769)
[PASS] testBenchmark_overheadGasUsage() (gas: 86218)
Logs:
  Overhead gas usage: 101252

[PASS] testHandle() (gas: 132010)
[PASS] testRemoteTransfer() (gas: 349557)
[PASS] testTransfer_withHookSpecified() (gas: 285463)
Suite result: ok. 5 passed; 0 failed; 0 skipped; finished in 9.95ms (1.97ms CPU time)

Ran 9 tests for test/token/HypERC20.t.sol:HypERC20Test
[PASS] testBenchmark_overheadGasUsage() (gas: 81052)
Logs:
  Overhead gas usage: 72667

[PASS] testDecimals() (gas: 15478)
[PASS] testInitialize_revert_ifAlreadyInitialized() (gas: 47199)
[PASS] testLocalTransfers() (gas: 85140)
[PASS] testRemoteTransfer() (gas: 284422)
[PASS] testRemoteTransfer_invalidAmount() (gas: 133123)
[PASS] testRemoteTransfer_withCustomGasConfig() (gas: 365775)
[PASS] testTotalSupply() (gas: 17557)
[PASS] testTransfer_withHookSpecified() (gas: 276380)
Suite result: ok. 9 passed; 0 failed; 0 skipped; finished in 9.99ms (3.63ms CPU time)

Ran 4 tests for test/token/HypERC20.t.sol:HypXERC20Test
[PASS] testBenchmark_overheadGasUsage() (gas: 77201)
Logs:
  Overhead gas usage: 68772

[PASS] testHandle() (gas: 59901)
[PASS] testRemoteTransfer() (gas: 337487)
[PASS] testTransfer_withHookSpecified() (gas: 272448)
Suite result: ok. 4 passed; 0 failed; 0 skipped; finished in 9.95ms (1.94ms CPU time)
| ../node_modules/@openzeppelin/contracts/proxy/transparent/TransparentUpgradeableProxy.sol:TransparentUpgradeableProxy contract |                 |        |        |        |         |
|--------------------------------------------------------------------------------------------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                                                                                                                | Deployment Size |        |        |        |         |
| 919654                                                                                                                         | 4816            |        |        |        |         |
| Function Name                                                                                                                  | min             | avg    | median | max    | # calls |
| balanceOf                                                                                                                      | 1240            | 2332   | 1240   | 9740   | 27      |
| decimals                                                                                                                       | 7373            | 7373   | 7373   | 7373   | 1       |
| enrollRemoteRouter                                                                                                             | 35899           | 82307  | 100132 | 120272 | 78      |
| handle                                                                                                                         | 65092           | 65092  | 65092  | 65092  | 19      |
| initialize                                                                                                                     | 34156           | 34156  | 34156  | 34156  | 1       |
| setDestinationGas                                                                                                              | 54032           | 54032  | 54032  | 54032  | 1       |
| setHook                                                                                                                        | 38701           | 38701  | 38701  | 38701  | 1       |
| totalSupply                                                                                                                    | 9494            | 9494   | 9494   | 9494   | 1       |
| transfer                                                                                                                       | 58310           | 58310  | 58310  | 58310  | 10      |
| transferRemote(uint32,bytes32,uint256)                                                                                         | 31522           | 113234 | 142723 | 165458 | 3       |
| transferRemote(uint32,bytes32,uint256,bytes,address)                                                                           | 135457          | 135457 | 135457 | 135457 | 1       |


| contracts/test/ERC20Test.sol:ERC20Test contract |                 |       |        |       |         |
|-------------------------------------------------|-----------------|-------|--------|-------|---------|
| Deployment Cost                                 | Deployment Size |       |        |       |         |
| 867167                                          | 4626            |       |        |       |         |
| Function Name                                   | min             | avg   | median | max   | # calls |
| allowance                                       | 2778            | 2778  | 2778   | 2778  | 1       |
| approve                                         | 46247           | 46247 | 46247  | 46247 | 7       |
| balanceOf                                       | 2561            | 2561  | 2561   | 2561  | 9       |
| transfer                                        | 51172           | 51252 | 51172  | 51400 | 17      |


| contracts/test/ERC20Test.sol:FiatTokenTest contract |                 |       |        |       |         |
|-----------------------------------------------------|-----------------|-------|--------|-------|---------|
| Deployment Cost                                     | Deployment Size |       |        |       |         |
| 981809                                              | 5170            |       |        |       |         |
| Function Name                                       | min             | avg   | median | max   | # calls |
| approve                                             | 46248           | 46248 | 46248  | 46248 | 2       |
| balanceOf                                           | 2583            | 2583  | 2583   | 2583  | 2       |
| transfer                                            | 51172           | 51286 | 51286  | 51400 | 8       |


| contracts/test/ERC20Test.sol:XERC20LockboxTest contract |                 |     |        |     |         |
|---------------------------------------------------------|-----------------|-----|--------|-----|---------|
| Deployment Cost                                         | Deployment Size |     |        |     |         |
| 2168698                                                 | 11966           |     |        |     |         |
| Function Name                                           | min             | avg | median | max | # calls |
| ERC20                                                   | 236             | 236 | 236    | 236 | 5       |


| contracts/test/ERC20Test.sol:XERC20Test contract |                 |       |        |       |         |
|--------------------------------------------------|-----------------|-------|--------|-------|---------|
| Deployment Cost                                  | Deployment Size |       |        |       |         |
| 1017277                                          | 5336            |       |        |       |         |
| Function Name                                    | min             | avg   | median | max   | # calls |
| allowance                                        | 2778            | 2778  | 2778   | 2778  | 1       |
| approve                                          | 46247           | 46247 | 46247  | 46247 | 2       |
| balanceOf                                        | 2539            | 2539  | 2539   | 2539  | 2       |
| transfer                                         | 51172           | 51286 | 51286  | 51400 | 8       |


| contracts/test/TestInterchainGasPaymaster.sol:TestInterchainGasPaymaster contract |                 |     |        |     |         |
|-----------------------------------------------------------------------------------|-----------------|-----|--------|-----|---------|
| Deployment Cost                                                                   | Deployment Size |     |        |     |         |
| 1675895                                                                           | 7980            |     |        |     |         |
| Function Name                                                                     | min             | avg | median | max | # calls |
| gasPrice                                                                          | 272             | 272 | 272    | 272 | 3       |


| contracts/test/TestMailbox.sol:TestMailbox contract |                 |       |        |       |         |
|-----------------------------------------------------|-----------------|-------|--------|-------|---------|
| Deployment Cost                                     | Deployment Size |       |        |       |         |
| 2015535                                             | 9329            |       |        |       |         |
| Function Name                                       | min             | avg   | median | max   | # calls |
| localDomain                                         | 250             | 250   | 250    | 250   | 68      |
| setDefaultHook                                      | 49862           | 49862 | 49862  | 49862 | 34      |
| setRequiredHook                                     | 49840           | 49840 | 49840  | 49840 | 34      |


| contracts/test/TestPostDispatchHook.sol:TestPostDispatchHook contract |                 |      |        |      |         |
|-----------------------------------------------------------------------|-----------------|------|--------|------|---------|
| Deployment Cost                                                       | Deployment Size |      |        |      |         |
| 242338                                                                | 902             |      |        |      |         |
| Function Name                                                         | min             | avg  | median | max  | # calls |
| messageDispatched                                                     | 516             | 516  | 516    | 516  | 6       |
| quoteDispatch                                                         | 871             | 1483 | 871    | 2871 | 49      |


| contracts/token/HypERC20.sol:HypERC20 contract       |                 |        |        |        |         |
|------------------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                                      | Deployment Size |        |        |        |         |
| 2940152                                              | 13947           |        |        |        |         |
| Function Name                                        | min             | avg    | median | max    | # calls |
| balanceOf                                            | 637             | 1007   | 637    | 2637   | 27      |
| decimals                                             | 273             | 273    | 273    | 273    | 1       |
| enrollRemoteRouter                                   | 7224            | 53737  | 71697  | 91597  | 78      |
| handle                                               | 35761           | 35761  | 35761  | 35761  | 19      |
| initialize                                           | 3853            | 173119 | 172894 | 192780 | 44      |
| setDestinationGas                                    | 25281           | 25281  | 25281  | 25281  | 1       |
| setHook                                              | 10181           | 10181  | 10181  | 10181  | 1       |
| totalSupply                                          | 2394            | 2394   | 2394   | 2394   | 1       |
| transfer                                             | 29788           | 29788  | 29788  | 29788  | 10      |
| transferRemote(uint32,bytes32,uint256)               | 2838            | 84561  | 114055 | 136790 | 3       |
| transferRemote(uint32,bytes32,uint256,bytes,address) | 106135          | 106135 | 106135 | 106135 | 1       |


| contracts/token/HypERC20Collateral.sol:HypERC20Collateral contract |                 |        |        |        |         |
|--------------------------------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                                                    | Deployment Size |        |        |        |         |
| 2347681                                                            | 11219           |        |        |        |         |
| Function Name                                                      | min             | avg    | median | max    | # calls |
| balanceOf                                                          | 27041           | 27041  | 27041  | 27041  | 5       |
| enrollRemoteRouter                                                 | 113213          | 113213 | 113213 | 113213 | 6       |
| handle                                                             | 62448           | 62448  | 62448  | 62448  | 1       |
| setDestinationGas                                                  | 46873           | 46873  | 46873  | 46873  | 1       |
| setHook                                                            | 48746           | 48746  | 48746  | 48746  | 1       |
| transferRemote(uint32,bytes32,uint256)                             | 28570           | 112931 | 144801 | 165422 | 3       |
| transferRemote(uint32,bytes32,uint256,bytes,address)               | 135403          | 135403 | 135403 | 135403 | 1       |


| contracts/token/HypNative.sol:HypNative contract     |                 |        |        |        |         |
|------------------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                                      | Deployment Size |        |        |        |         |
| 2140696                                              | 10133           |        |        |        |         |
| Function Name                                        | min             | avg    | median | max    | # calls |
| balanceOf                                            | 21705           | 21705  | 21705  | 21705  | 1       |
| enrollRemoteRouter                                   | 113191          | 113191 | 113191 | 113191 | 6       |
| handle                                               | 60914           | 60914  | 60914  | 60914  | 1       |
| setDestinationGas                                    | 46851           | 46851  | 46851  | 46851  | 1       |
| setHook                                              | 48746           | 48746  | 48746  | 48746  | 1       |
| transferRemote(uint32,bytes32,uint256)               | 22041           | 98018  | 125697 | 146318 | 3       |
| transferRemote(uint32,bytes32,uint256,bytes,address) | 116189          | 116189 | 116189 | 116189 | 1       |


| contracts/token/extensions/HypFiatToken.sol:HypFiatToken contract |                 |        |        |        |         |
|-------------------------------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                                                   | Deployment Size |        |        |        |         |
| 2367920                                                           | 11324           |        |        |        |         |
| Function Name                                                     | min             | avg    | median | max    | # calls |
| balanceOf                                                         | 27063           | 27063  | 27063  | 27063  | 2       |
| enrollRemoteRouter                                                | 113213          | 113213 | 113213 | 113213 | 4       |
| handle                                                            | 29923           | 45167  | 44240  | 61340  | 3       |
| transferRemote(uint32,bytes32,uint256)                            | 149951          | 149951 | 149951 | 149951 | 1       |
| transferRemote(uint32,bytes32,uint256,bytes,address)              | 140553          | 140553 | 140553 | 140553 | 1       |


| contracts/token/extensions/HypXERC20.sol:HypXERC20 contract |                 |        |        |        |         |
|-------------------------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                                             | Deployment Size |        |        |        |         |
| 2148777                                                     | 10292           |        |        |        |         |
| Function Name                                               | min             | avg    | median | max    | # calls |
| balanceOf                                                   | 27019           | 27019  | 27019  | 27019  | 2       |
| enrollRemoteRouter                                          | 113213          | 113213 | 113213 | 113213 | 4       |
| handle                                                      | 44097           | 52647  | 52647  | 61197  | 2       |
| transferRemote(uint32,bytes32,uint256)                      | 140968          | 140968 | 140968 | 140968 | 1       |
| transferRemote(uint32,bytes32,uint256,bytes,address)        | 131570          | 131570 | 131570 | 131570 | 1       |


| contracts/token/extensions/HypXERC20Lockbox.sol:HypXERC20Lockbox contract |                 |        |        |        |         |
|---------------------------------------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                                                           | Deployment Size |        |        |        |         |
| 2671362                                                                   | 13199           |        |        |        |         |
| Function Name                                                             | min             | avg    | median | max    | # calls |
| balanceOf                                                                 | 27018           | 27018  | 27018  | 27018  | 4       |
| enrollRemoteRouter                                                        | 113235          | 113235 | 113235 | 113235 | 5       |
| handle                                                                    | 79997           | 86837  | 86837  | 93677  | 2       |
| lockbox                                                                   | 294             | 294    | 294    | 294    | 2       |
| transferRemote(uint32,bytes32,uint256)                                    | 200300          | 200300 | 200300 | 200300 | 1       |
| transferRemote(uint32,bytes32,uint256,bytes,address)                      | 192780          | 192780 | 192780 | 192780 | 1       |
| wrappedToken                                                              | 271             | 271    | 271    | 271    | 1       |
| xERC20                                                                    | 295             | 295    | 295    | 295    | 3       |




Ran 6 test suites in 60.47ms (59.44ms CPU time): 34 tests passed, 0 failed, 0 skipped (34 total tests)
