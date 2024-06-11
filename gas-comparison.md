# Gas Comparison

The gas needed to wrap token and before calling the bridge relaying logic

| Project       | Gas used|
|---------------|---------|
| xERC20        | 270,238 |
| Warp Route    | 258,099 |
| Omnibridge*   | 225,920 |
| SJ* Token     | 157,802 |


* Include the bridge relaying logic

### Reference
1. [xERC20](./xERC20.md): `E2ELockbox::testDeposit()`
2. [HypERC20](./HypERC20_no_handle.md): `HypERC20CollateralTest::testRemoteTransfer()`
3. [Omnibridge](https://dashboard.tenderly.co/tx/mainnet/0xc8e4e4a735d60bab6265bff2081f707c1996cfa1804a414c38c084ffb94ef4ad/gas-usage)
4. [SJ* Token](SJToken.md)