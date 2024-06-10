# Connext xERC20 Gas Report

Run test from https://github.com/defi-wonderland/xERC20/blob/main/solidity/test/e2e/XERC20Lockbox.sol

## Gas report

yarn run v1.22.15
$ forge test --match-contract E2E -vvv --via-ir --gas-report
No files changed, compilation skipped

Ran 2 tests for solidity/test/e2e/XERC20.t.sol:E2EMintAndBurn
[PASS] testBurn() (gas: 375807)
[PASS] testMint() (gas: 232980)
Suite result: ok. 2 passed; 0 failed; 0 skipped; finished in 637.50ms (1.58ms CPU time)

Ran 2 tests for solidity/test/e2e/XERC20Factory.t.sol:E2EDeployment
[PASS] testDeploy() (gas: 40013)
[PASS] testDeployLockbox() (gas: 2630078)
Suite result: ok. 2 passed; 0 failed; 0 skipped; finished in 642.55ms (5.49ms CPU time)

Ran 4 tests for solidity/test/e2e/XERC20Lockbox.sol:E2ELockbox
[PASS] testDeposit() (gas: 270238)
[PASS] testDepositTo() (gas: 272416)
[PASS] testLockbox() (gas: 10824)
[PASS] testWithdraw() (gas: 360988)
Suite result: ok. 4 passed; 0 failed; 0 skipped; finished in 642.56ms (15.31ms CPU time)

Ran 14 tests for solidity/test/e2e/XERC20.t.sol:E2EParameterMath
[PASS] testAddingMintersAndLimits() (gas: 633684)
[PASS] testChangeLimit() (gas: 218555)
[PASS] testChangingMaxLimitUpdatesCurrentLimit() (gas: 283560)
[PASS] testChangingMaxLimitWhenLimitIsUsedUpdatesCurrentLimit() (gas: 437246)
[PASS] testChangingPartialMaxLimitUpdatesCurrentLimitWhenUsed() (gas: 455825)
[PASS] testChangingPartialMaxLimitUpdatesCurrentLimitWithIncrease() (gas: 455953)
[PASS] testCurrentLimitIsMaxAfterDuration() (gas: 378084)
[PASS] testCurrentLimitIsSameIfUnused() (gas: 219621)
[PASS] testCurrentLimitIsUpdatedWithTime() (gas: 406491)
[PASS] testMultipleBridgesBurnsHaveDifferentValues() (gas: 797562)
[PASS] testMultipleBridgesHaveDifferentValue() (gas: 775056)
[PASS] testMultipleMintsAndBurns() (gas: 1101980)
[PASS] testMultipleUsersUseBridge() (gas: 574961)
[PASS] testUseLimitsUpdatesLimit() (gas: 378312)
Suite result: ok. 14 passed; 0 failed; 0 skipped; finished in 642.61ms (28.00ms CPU time)
| solidity/contracts/XERC20.sol:XERC20 contract |                 |        |        |        |         |
|-----------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                               | Deployment Size |        |        |        |         |
| 0                                             | 0               |        |        |        |         |
| Function Name                                 | min             | avg    | median | max    | # calls |
| FACTORY                                       | 287             | 287    | 287    | 287    | 1       |
| approve                                       | 26104           | 44898  | 46004  | 46004  | 18      |
| balanceOf                                     | 687             | 687    | 687    | 687    | 5       |
| burn                                          | 44976           | 50463  | 46614  | 56864  | 16      |
| burningCurrentLimitOf                         | 1269            | 1538   | 1597   | 1597   | 16      |
| burningMaxLimitOf                             | 935             | 1435   | 935    | 2935   | 4       |
| mint                                          | 65715           | 74741  | 78015  | 82815  | 22      |
| mintingCurrentLimitOf                         | 1087            | 1363   | 1415   | 1415   | 18      |
| mintingMaxLimitOf                             | 451             | 736    | 451    | 2451   | 7       |
| name                                          | 2896            | 2896   | 2896   | 2896   | 1       |
| owner                                         | 2657            | 2657   | 2657   | 2657   | 24      |
| setLimits                                     | 57333           | 178360 | 204735 | 204735 | 24      |
| symbol                                        | 3312            | 3312   | 3312   | 3312   | 1       |
| totalSupply                                   | 343             | 343    | 343    | 343    | 1       |


| solidity/contracts/XERC20Factory.sol:XERC20Factory contract |                 |         |         |         |         |
|-------------------------------------------------------------|-----------------|---------|---------|---------|---------|
| Deployment Cost                                             | Deployment Size |         |         |         |         |
| 3830824                                                     | 17656           |         |         |         |         |
| Function Name                                               | min             | avg     | median  | max     | # calls |
| deployLockbox                                               | 747522          | 763878  | 764622  | 764622  | 23      |
| deployXERC20                                                | 1872286         | 2063602 | 2072299 | 2072299 | 23      |


| solidity/contracts/XERC20Lockbox.sol:XERC20Lockbox contract |                 |        |        |        |         |
|-------------------------------------------------------------|-----------------|--------|--------|--------|---------|
| Deployment Cost                                             | Deployment Size |        |        |        |         |
| 0                                                           | 0               |        |        |        |         |
| Function Name                                               | min             | avg    | median | max    | # calls |
| ERC20                                                       | 304             | 304    | 304    | 304    | 3       |
| XERC20                                                      | 260             | 260    | 260    | 260    | 3       |
| deposit                                                     | 104655          | 104655 | 104655 | 104655 | 2       |
| depositTo                                                   | 105147          | 105147 | 105147 | 105147 | 1       |
| withdraw                                                    | 65180           | 65180  | 65180  | 65180  | 1       |




Ran 4 test suites in 685.96ms (2.57s CPU time): 22 tests passed, 0 failed, 0 skipped (22 total tests)
Done in 1.15s.
