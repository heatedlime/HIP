# HIP XX: MOBILE NFT Creation Fee
- Author(s): [Andy Zyvoloski](https://github.com/heatedlime) & [Keith Rettig](https://github.com/keithrettig)
- Start Date: 
- Category: Economic
- Original HIP PR: 
- Tracking Issue:
- Voting Mechanism: veMOBILE

## Summary:
This HIP requires the creation and holding of a non-fungible token (NFT) for devices that do not pay an onboarding fee on the MOBILE subDAO. Whichever wallet holds the NFT will receive applicable MOBILE rewards for that device. NFTs for active devices will vary in range, and the NFT Creation burn fee is noted in the detailed explanation section below. 

As this HIP creates moves radios on chain in the form of NFTs, this HIP also changes the rewardable entity of MOBILE from MOBILE Hotspots to radios.

## Motivation:
When the MOBILE token was first premined and distributed in August 2022, it had no source of backing, such as HNT. As part of the Solana migration in April 2023, the MOBILE subDAO treasury was established and the treasury swap function was created making it possible to swap MOBILE for HNT within the MOBILE subDAO treasury. However, since eight (8) months of MOBILE rewards aggregating over 30 Billion MOBILE were distributed with no backing in HNT, the redemption rate for MOBILE within the MOBILE subDAO treasury is extremely undersized. To increase the redemption rate, one of two things must happen:

1. The daily amount of HNT distributed to the MOBILE subDAO treasury must increase; however, this is limited as these emissions are also shared with the IOT subDAO; or, 
2. The amount of outstanding MOBILE needs to decrease (i.e. burn).

This HIP aims to address number 2 above by decreasing the overall supply of MOBILE as by implementing a new rewardable NFT creatuib fee fir devices that are added to the network that do not occur an onboarding fee. 

## Stakeholders:

Service Provider Subscriber will be required to custody an NFT linked to their SP Subscriber account in order to earn DNT from a rewardable event, such as Discover Mapping. 

Service Providers (SP) will be required to burn the MOBILE tokens to create a Subscriber NFT for each of their subscribers that enable Discover Mapping mode.

Current and Future Radios and or Carrier Offload Wi-Fi devices will be required to pay NFT creation fees.

MOBILE token holders will benefit from this HIP as the burning of MOBILE tokens will decrease the total supply.

Device Manufacturers are recommended to prepay the MOBILE NFT creation fee to help ensure a smoth onboarding process


## Detailed Explanation:

This HIP proposes requiring all active devices that are not required to pay an onboard fee to be stored on chain via an NFT, and pay a NFT creation fee by burining MOBILE. The following amount of MOBILE is to be burned for the creation of a rewardable NFT for the following active devices:


| Active Device                     | MOBILE Burn Fee|  
|-----------------------------------|----------------|
|Service Provider Discovery Mapping | $5.00          |
|Indoor Wi-Fi                       | $5.00          |
|Physcial SPOT Mapper               | $10.00         |
|Indoor Radio                       | $10.00         |
|Outdoor Wi-Fi                      | $20.00         |
|Outdoor Low Power Radio            | $25.00         |
|Outdoor High Power Radio (436h)    | $50.00         |

Note, that if any of the Active Devices listed above ever require an onboarding fee, the onboarding fee will superceed the MOBILE burn fee, and an NFT will be created at the time of onboarding, which will be covered by the onboarding fee. 

## Active Device Details

### Service Provider Discovery Mapping NFTs
A Subscriber NFT will be required in order for Service Provider subscribers to be rewarded in the subDAO’s Decentralized Network Tokens (DNT) for rewardable events, such as Discovery Mapping.  The creation of the NFT is to be paid for by the Service Provider; it is the option of the Service Provider if they wish to pass the cost through to their Subscriber.  The specific definitions and reward values of Rewardable Events are the responsibility and liability of the Service Provider. This HIP also requires that a Service Provider must have already staked the 500M MOBILE required to become a Service Provider prior to creatining any NFTs.

The burning of MOBILE will be required in order to create the Subscriber NFT, thus, the NFT cannot be created until the appropriate amount of MOBILE is burned. If Discovery Mapping for Service Provider Subscribers is released prior to the implementation of this HIP, this HIP requires that each Service Provider retroactively burn the appropriate amount of MOBILE based on the price of MOBILE the day the retroactive burn is paid. Once a burn method and NFT creation process is created as noted in Phase 1 below, Service Providers will have 90 calendar days to retroactively burn all applicable MOBILE. If the burn is not paid by the 91st calendar day after the completion on Phase 1, Discovery Mapping must be turned off for ALL subscribers for that Service Provider until the burn is paid in full. If Discover Mapping is not turned off on the 91st calendar day after Phase 1 completion, the Service Provider will be penalized by 250,000 MOBILE every day it is not turned off, or paid in full. This penalty will be directly taken and burned from the Service Providers Initial Stake of 500M MOBILE. 

There may be instances in which a Subscribers NFT accidently gets lost, stolen, or burned. Therefore, this HIP will allow the SP to create a new Subscriber NFT for that subscriber, with an additional MOBILE burn at the same cost in the pricing schedule above. The SP will be responsible for verifying the identity of the subscriber prior to the minting of a new NFT. This fee may be passed on to the Subscriber by the SP.

#### Physical SPOT Mapper (or similar device)
The SPOT Mapper is a physical handheld device that is used to map multiple Helium DAO sub networks, such as MOBILE, IOT, etc. Therefore, this device may be be used on multiple networks. In order to earn rewards for mapping the MOBILE network, the NFT creation fee will need to be paid, as described in the pricing schedule above. It is suggested that manufactures selling these devices prepay for the onboard fee of these devices to simplify the consumer onboarding process.

### CBRS Radios
At the time of this HIP, there have been more than 10,000 CBRS radios onboarded to the MOBILE subDAO. This HIP will require radio owners to retroactively burn the NFT creation fee for their radios in order to keep earning MOBILE. A 90 day grace period will be given after the Phase 3 process, noted below, is implemented to burn MOBILE and create an NFT. It is suggested that manufactures selling these devices prepay for the onboard fee of these devices to simplify the consumer onboarding process.

### Carrier Offload Wi-Fi (CoWi-FI)
At the time of this HIP, CoWi-FI units had yet to be released for public sale. If this HIP is implemented prior to the release of these devices, it is recommended that manufactures selling these devices prepay for the onboard fee of these devices to simplify the consumer onboarding process. If these devices are onboarded to the network prior to the implementation of this HIP, all CoWi-FI device owners will be required to retroactively pay the NFT creation fee for their devices in order to keep earning MOBILE. A 90 day grace period will be given after the process to burn MOBILE and create an NFT is implemented. 

## Drawbacks:
Similar to how NFTs work for the IOT subDAO, if an NFT for a IOT Hotspot is lost, accidently burned, or stolen, Radio, CoWi-FI and Spot Mapper devices will also be unable to create a new NFT for that device. 

## Alternatives:
An alternative can be to keep active devices stored off chain, and continue to have the rewardable entity MOBILE Hotspots. 

## Unresolved Questions:
Should the amount be linked to a fiat value, or defined value of MOBILE?

### Implementation Phases
This HIP suggests this HIP is implemented in the phases noted below.

#### Phase 1 - NFT Creation for Service Provider Discovery Mapping Rewards
The MOBILE community requests that the Helium Foundation and or Nova Labs create a method to permanently burn MOBILE in exchange for a rewardable NFT for Service Provider Subscribers. Additionally, a way to reward NFT holders will need to be created.

#### Phase 2 - NFT Creation for Service Provider CoWi-FI devices
The MOBILE community requests that the Helium Foundation and or Nova Labs create a method to permanently burn MOBILE in exchange for a rewardable NFT for CoWi-Fi devices. Additionally, a way to reward NFT holders will need to be created.

#### Phase 3
The MOBILE community requests that the Helium Foundation and or Nova Labs create a method to permanently burn MOBILE in exchange for a rewardable NFT for Radio devices. The switch from rewarding MOBILEL Hotspots to Radios will need to be implemented. 
