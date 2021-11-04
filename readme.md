# Donkey Staking
## Description
VDON StakingContract allows users to stake their DON tokens for a predetermined term in exchange for VDON tokens and interest (in the form of DON and ecoCNG tokens). As of Friday (11/04 KST), ownership of VDON tokens will grant users exclusive rights including but not limited to voting/submitting governance proposals and claiming a certain portion of Donkey Protocols' revenue.
In future updates, as part of an effort to promote Donkey Protocol's token economy and incentivize users to hold on to their VDON tokens, the team will be extending VDON tokens' utilities so that VDON holders can enjoy a more varied form of exclusive benefits.
## Error code  

E1
- revert when unauthorized

E67
- revert when reentered

E80
- revert when transferIn overflow

E81
- revert when transferOut failed

E101
- revert when `mintAmount` is equal to or below zero

E102
- revert when the same timestamp exists in `stakingProductOf[acocunt]`

E103
- revert when `expectedTotalInterest` exceeds `interestLimitAmount`

E104
- revert when user has not enough balance to mint

E105
- revert when `claimDonBehalf` fails

E106
- revert when trying to redeem product which has principal equal or below zero

E107
- revert in `redeem` when current block.timestamp < relaseTime

E108
- revert in `redeem`, `redeemPrincipal` when contract has insufficient balance to transfer

E109
- revert when user request empty staking product

E112
- revert when trying to delete product even though user has no entered product

E113
- revert when idx value is invalid

## Attribution

Some of this codebase is modified from existing works, including:

[Compound](https://github.com/compound-finance)  
[OpenZepplin](https://github.com/OpenZeppelin)


> refers to [Donkey License](https://docs.donkey.fund/about/security)

## License

### BSD 3-Clause "New" or "Revised" License
> A permissive license similar to the BSD 2-Clause License, but with a 3rd clause that prohibits others from using the name of the project or its contributors to promote derived products without written consent.


```
Copyright 2021 Donkey

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```