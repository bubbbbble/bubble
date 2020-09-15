# [中文版](https://github.com/bubbbbble/bubble/blob/master/READMECN.md)

# About Bubble

Bubble is a token protocol that provides value support through Ethereum incentives. Staking BUB can get higher ETH reward, and the increase in ETH reward will in turn provide stronger support for the value of BUB. In addition, Bubble incorporates multiple coefficients to boost ROI, which means you can control your own earnings . However, as the name of Bubble implies, Bubble's token economy is a bubble experiment.
So, can you get what you eager for on Bubble?
Good Luck!


> **Token symbol： BUB**

> **Token type： ERC-20**

> **Token Supply： 100,000,000**


## Distribution

Pool|Quantity|Percentage|Description
---|:--:|:--|:--
initial liquidity|200,000|0.2%|Add Uniswap liquidity injection
BUB Pool|96,000,000|96%|BUB mining distribution
Referral Pool|2,000,000|2%|Referral rewards
Prize Pool|1,800,000|1.8%|It will be released in 10 rounds based on the prize pool balance, and the released BUB will be converted into ETH to recharge into the prize pool (see the table below for details)
Total|100,000,000|100%            

## Release Ratio

Round|1st round|2st round|3st round|4st round|5st round|6st round|7st round|8st round|9st round|10st round
---|:--|:--|:--|:--|:--|:--|:--|:--|:--|:--
Prize pool balance（ETH）|100|150|200|250|300|400|500|600|700|800
Release ratio|10%|10%|10%|10%|10%|10%|10%|10%|10%|10%


# Mining Details

* There are 3 mining pools: ETH pool, BUB pool, and referral pool. You need to start with ETH pool to activate the other two pools. 
* Mining ROI = basic ROI *coefficients  

## Coefficients List


* 1.Mine Owner Level Coefficient: Calculate the level and coefficient based on the amount of ETH staked for mining. 


Mine owner level|LV1|LV2|LV3
---|:--|:--|:--
The amount of staked ETH|1-5|6-10|>=11
Coefficients|0.3|0.6|1


* 2.Mining Boost Coefficient: calculate the level and coefficient based on Boost level.


Boost level|LV1|LV2|LV3|LV4|LV5|LV6 
---|:--|:--|:--|:--|:--|:--
The amount of staked BUB|400|1,500|2,000|8,000|40,000|200,000 
Mining Boost Coefficients|1.5|1.7|2|2|2|2



* 3.Re-investment Coefficient: A coefficient calculated based on the times of re-investment, any withdrawal operation will reset your times of re-invesment. 


The number of re-investment|0 times|1 times|2 times|3 times|4 times and above
---|:--|:--|:--|:--|:--
Coefficients|1.0|1.3|1.7|2.2|3


* 4.Genesis Boost: Rewards settled within 14 days after contract deployment will enjoy genesis boost with a coefficient of 2. 

# About Mining

* Lock-up Period: The staked principal has a default lock-up period of 5 days. After the stake is released, the profit will not be calculated and can be withdrawn at any time. After the withdrawal, the reward for referral will not be calculated.
 
* Withdrawal: You can withdraw the token in the withdrawable amount at any time. If you are staking token, you can withdraw the token after the lock-up expires (note: any withdrawal operation will reset the number of reinvestments).




* Staking Buffer: After you complete the first stake, the contract will start to calculate the lock-up time. 12 hours after the start time of stake is the buffer period. During this period you can continue to stake, but the lock-up time will be recalculated.

	
* Re-investment Boost: Every time you add a re-investment, your re-investment coefficient will increase. The staking buffer period will also start after the re-investment.

## 1.ETH Pool

* Mining Method: get extra ETH as a reward by staking your ETH.

* Staking Limit per Round: Above 1 ETH

* Mine Owner Level: The one who stake 1-5 ETH is the LV1, the 6-10 ETH is the LV2, and above 11 ETH is the LV3.

* Basic ROI : 0.3% per day, APY 109.5% 

* Calculation: Total Yield / Round = basic ROI * genesis boost * mine owner level coefficient * mining boost coefficient * re-investment coefficient*5 (days)


> For example: You start mining for the first time during the genesis period, staked 15 ETH and 10,000 BUB at the same time, the 5-day ETH income will be 15 * 0.3% * 2 * 1.0 * 2.0 * 1.0 * 5 = 0.9 ETH, APY is as high as 438%; if you chooses to continue reinvesting in the 2nd round, the return will be 0.9 * 1.3 = 1.17 ETH, and the APY will increase to 569.4%.


## 2.BUB Pool

* Mining Method: get extra BUB as a reward by staking your BUB.

* Basic ROI : 15% per round, APY 1095%

* You need to start ETH mining first, then you can stake BUB.

* Calculation: Total Yield / Round = basic ROI * genesis boost * mine owner level coefficient * re-investment coefficient

> For example: You started mining for the first time during the genesis period, staked 15 ETH and 20,000 BUB at the same time. After 5 days, the profit will be 15,000 * 15% * 2 * 1.0 * 1.0 = 2,250 BUB, the APY is as high as 2190%.


## 3.Referral Pool


* Mining Method: get BUB and ETH rewards by inviting friends to staking in the ETH pool.

* BUB Rewards: Every time the invitee starts a round of ETH mining, the inviter will receive a fixed BUB reward.


Mine owner level of invitee|LV1|LV2|LV3
---|:--|:--|:--
BUB rewards for inviter|200|600|1,000


* ETH Rewards: The basic return is 50% of the ETH mining reward of the invitee, and the boost coefficient of the referral level is as follows: 

`Referral Boost Coefficient: calculate the level and coefficient based on Boost level.`

Boost level|LV1|LV2|LV3|LV4|LV5|LV6
---|:--|:--|:--|:--|:--|:--
The amount of staked BUB|400|1,500|2,000|8,000|40,000|200,000
Referral boost Coefficients|1|1|1|1.2|1.5|2


* Calculation: Total Earnings=50% * ETH mining reward of the invitee * mine owner level coefficient * Referral boost coefficient + BUB rewards

> For example: You referred A, and you staked 15 ETH and 15,000 BUB for mining. During your mining period, A also invested 15 ETH for mining, earning 0.2 ETH per day. Then, after 5 days, the referral rewards you can get are 50% * 0.2 * 5 * 1.0 * 1.2 = 0.6 ETH and 1,000 BUB.

# Prize Pool

* Source of Funding: 2% of the ETH pool deposit will be automatically transferred to the prize pool. The proportion will increase to 3% after 20 days of contract deployment, 4% after 30 days, and 5% after 40 days.In addition, 9,000,000 BUB will be released in 10 rounds based on the prize pool balance, and the released BUB will be converted into ETH to recharge into the prize pool. 

* Prize Pool Distribution: Your rank is based on your BUB share locked in the prize pool, and the top 5 will share all prize pool as follows: 1st place 52%,2nd place 23%,3rd place 14%,4th place 8% and 5th place 3%. 

* Draw: When contract balance of the ETH pool is 0, the system will lock the mining pool contract and start a 24-hour countdown. During the countdown, you can continue to stake BUB into the prize pool. After the countdown ends, the prize pool will be settled based on the latest ranking. 

* Protection Period: During 20 days of contract deployment, the draw will not be triggered when the ETH pool contract balance is 0.
 

# Others

* 5% of the ETH pool deposit will be automatically transferred to a special account, of which 3% is used for application development and 2% is used for team operations.

* Restart: After the prize pool is drawn, the system will restart, and deploy a new contract.
 









