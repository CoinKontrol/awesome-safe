# Awesome Safe

This repository contains a curated list of resources related to SAFE smart 
account wallet. The list is designed to help developers and integrators build 
on top of Safe, integrate Safe into their applications or develop Safe modules.

🚧 This is a work in progress and many of the modules have not been curated. 
Contributions are welcomed - if you created or maitaining any of the modules in this
list and would like to correct or add more details please make a PR to this repo 🚧

## Safe Modules

Modules that are available open source

### ERC-7579 Modules

[ERC-7579](https://docs.safe.global/advanced/erc-7579/overview) is a standard for smart accounts modules. 

### Zodiac Compatible

Zodiac is an [open standard](https://eips.ethereum.org/EIPS/eip-5005) for building modular accounts focusing on DAO tooling.

* [snapshot zodiac module](https://github.com/tellor-io/snapshot-zodiac-module/tree/tellor)
    * Allows on-chain execution based on the outcome of Snapshot proposals reported by Tellor oracle
    
* [bridge module](https://github.com/gnosisguild/zodiac-module-bridge)
    * This module allows the address on one chain to control a Safe on a different chain
    using Arbitrary Message Bridge
    * [wiki](https://zodiac.wiki/index.php%3Ftitle=Category:Bridge_Module.html)

* [conext zodiac module](https://github.com/gnosisguild/zodiac-module-connext)
    * This module allows a function call from a different chain or rollup to a Safe
    via the Connext bridge.

* [exit module](https://github.com/gnosisguild/zodiac-module-exit)
    * This module allows participants to redeem a designated token for a 
    proportional share of an avatar's digital assets, similar to Moloch DAO's 
    rageQuit() function.
    * [wiki](https://zodiac.wiki/index.php%3Ftitle=Category:Exit_Module.html)

* [governor module](https://github.com/gnosisguild/zodiac-module-oz-governor)
    * The OZ Governor Module is an opinionated implementation of OpenZeppelin's 
    Governor contracts designed to be used in a Zodiac-style setup, allowing a 
    Avatar (like a Gnosis Safe) to controlled by on-chain governance similar to 
    Compound's Governor Alpha and Bravo.
    * [wiki](https://zodiac.wiki/index.php%3Ftitle=Category:Governor_Module.html)

* [reality module](https://github.com/gnosisguild/zodiac-module-reality)
    * This module allows on-chain execution based on the outcome of events reported by Reality.eth
    * [wiki](https://zodiac.wiki/index.php%3Ftitle=Category:Reality_Module.html)\

* [zodiac module siphon](https://github.com/gnosisguild/zodiac-module-siphon)
    * This module exposes a public interface which allows anyone to trigger an 
    Avatar to withdraw from a designated liquidity position in order to pay down 
    some of its debt in a designated debt position, thereby improving the 
    health of the position.

* [zodiac delay modifier](https://github.com/gnosisguild/zodiac-modifier-delay)
    * Safe module that allows approved addresses to execute transactions after 
    a time delay, during which transactions can be marked as invalid by the Safe.
    * [wiki](https://zodiac.wiki/index.php%3Ftitle=Category:Delay_Modifier.html)

* [zodiac roles](https://github.com/gnosisguild/zodiac-modifier-roles)
    * This modifier allows avatars to enforce granular, role-based, permissions 
    for attached modules.
    * [wiki](https://zodiac.wiki/index.php%3Ftitle=Category:Roles_Modifier.html)

* [zodiac guard scope](https://github.com/gnosisguild/zodiac-guard-scope)
    * A transaction guard that allows the owner to limit the multisig signers 
    to calling specific function signatures on specific contracts.

* [zodiac guard mod](https://github.com/gnosisguild/zodiac-guard-mod)
    * A guard that prevents the contract its guarding from disabling protected 
    modules.

* [zodiac usul module](https://github.com/SekerDAO/Usul)
    * Zodiac module that allows a DAO to use various types of voting using Safes

* [moloch-safe-module](https://github.com/bitbeckers/moloch-safe-modules)
    * CookieJar is a module for a DAO (Decentralized Autonomous Organization) or similar type of organization, that allows certain members to make claims (potentially for funds or other assets) at certain intervals.

### Regular Modules

* [safe-module-claim-settlement](https://github.com/cardstack/safe-module-claim-settlement)
    * Safe module that enables a user to distribute crypto assets via meta transactions

* [passkey module](https://github.com/safe-global/safe-modules/tree/main/modules/passkey)
    * Module contains a passkey signature verifier, that can be used as an owner for a Safe, compatible with versions 1.3.0+.

* [4337 module](https://github.com/safe-global/safe-modules/tree/main/modules/4337)
    * Enable 4337 with a safe

* [allowances](https://github.com/safe-global/safe-modules/tree/main/modules/allowances)
    * Registry for transfer allowances (ERC20 and Ether)

* [safe minion](https://github.com/HausDAO/MinionSummonerV2/blob/main/contracts/SafeMinion.sol)
    * Allows a DAO to control treasury using a Safe
    * [wiki](https://daohaus.substack.com/p/6991f40b-3931-47ff-bea3-fa6f9c365135?s=r)

* [linkdrop safe module](https://github.com/LinkdropHQ/linkdrop-safe-module)
    * Linkdrop allows you to send tokens to anyone using a claim link. Behind this is a Safe with a custom module

* [cardstak meta guard](https://github.com/cardstack/cardstack-meta-guard)
    * A transaction guard that allows avatar or module to have multiple guards.

* [gelato safe module](https://github.com/gelatodigital/gelato-safe-module)
    * Gelato Safe Module to automate transactions for Gnosis Safe's Resources

* [safe flashloan](https://github.com/dialecticch/safe-flashloan)
    * Lend out all the assets in your Gnosis Safe for flashloans. This is 
    loosely based on the Aave implementation of flashloans.

* [revoke safe module](https://github.com/emilianobonassi/revoke-safe-module)
    * A Gnosis Safe Module to delegate to an another account to revoke on your 
    behalf token allowances for an exploited address.

* [safe vest module](https://github.com/Phala-Network/safe-vest-module)
    * A Gnosis Safe module that vest tokens periodically

* [gas saver safe module](https://github.com/emilianobonassi/gas-saver-gnosis-safe-module)
    * A collection of smart contracts to save gas on Ethereum in a Gnosis Safe 
    Wallet leveraging GST2 or CHI tokens

* [safe cross chain module](https://github.com/crosschain-alliance/safe-crosschain)
    * Simple module to control a Safe via crosschain calls with Hashi
    
* [wei roll safe module](https://github.com/weiroll/safe-module)
    * Weiroll is a scripting language for EVM. The SAFE module allows a Safe to specify users that can execute arbitrary scripts or users who can execute specific scripts on behalf of the Safe itself.

* [safe recovery module](https://github.com/bxmmm1/safe-recovery-module)
    * Social recovery module, [more info](https://forum.safe.global/t/social-recovery-module/2117)
    
* [safe recovery module 2](https://github.com/5afe/safe-recovery-module)
    * Using Safe transactions trusted addresses can be set as delegates and a recover period in seconds can be set. Any of the delegates' addresses can start the recovery process and finally recover the safe after the recover period has passed. During the recover period the recovery process can be stopped at any time using Safe transactions
  
* [safe module template](https://github.com/bxmmm1/safe-module-template)
    * Safe module template in Foundry
     
* [safe recovery modules](https://github.com/keviinfoes/Safe-recovery-modules)
   * Inheritance module
      * The inheritance module allows a SAFE to set new owners (heirs) with a time delay. The time delayed heirs can be
   * Secret recovery module
      * Secret recovery allows use of guardians with significant delays (for example years), minimizing trust, while allowing a reduction of this delay by revealing known secrets. Multiple secrets can be added eacht with a custom reduction period. Allowing users to choose between low entropy secrets that are easy to remember (with a smal delay reduction) and high entropy secrets with significant delay reduction (hard to remember).
  
* [safe module](https://github.com/compassdao/safe-module)
   * Similar to Zodiac roles, allows to set permissions 

* [safe syntethics module](https://github.com/Synthetixio/safe-synthetix-module)
   * Customization for Gnosis Safes used to govern Synthetix protocol

* [safe module](https://github.com/kotik98/safe-module)
   * This project contains module for gnosis safe wallet which allows to whitelist transactions (contract addresses, functions and arguments) and make these transactions without any additional signatures.

* [safe guard](https://github.com/withtally/safeguard)
   * Safeguard is a tool for on-chain Ethereum DAOs to delegate funds to multisigs while keeping some level of control

* [safe modules](https://github.com/vaporyorg/safe-modules)
   * Three old safe modules: Allowance Module, DutchX Seller Module and Recurring Transfers Module
   * These look like a fork / copy of the original safe modules that were found in the safe org

* [safe modules](https://github.com/Code-Connect-ETH/Safe-Module)
   * Allowance module

* [safe module](https://github.com/ninabarbakadze/safe-module)
   * Withdraw module allows accounts not related to the Safe to withdraw a predetermined amount of a specific token using alternative access scheme.
 
* [safe payouts module](https://github.com/czar0/safe-payouts-module)
   * Example of a Gnosis Safe module for company/DAO payouts written in Solidity

* [solace safe module](https://github.com/hwnprsd/solace-safe-module)
   * A set of contracts which helps SAFE Smart Accounts interface with the Solace Key Network

* [bico safe module](https://github.com/pythonpete32/bico-safe-module)
   * Gnosis safe module for claiming vested BICO tokens, and staking from a safe.

* [poc safe module](https://github.com/Bapi-Reddy/poc_safe_module)
   * A poc implementation of safe module, that takes a delta neutral(dn) position with glp and shorting proportional amounts on aave. It uses gelato tasks to maintain healthfactor at safe levels and rebalance the delta netural positions by adjusting short position on aave.

* [unicorn safe module](https://github.com/harry91198/UnicornSafeModule)
   * This project is a Safe Module implementation for a Safe contract to withdraw a predetermined amount of Unicorn token.

* [dagon safe module](https://github.com/jamesmccomish/dagon-safe-module)
   * This module is designed to enable a Safe to track the contributions of members by minting a Dagon token.    

* [token withdrawal module](https://github.com/roleengineer/token-withdrawal-module)
   * A Safe Module, which allows accounts that are not related to the Safe, to withdraw a predetermined amount of a specific token. 

* [safe module example faucet](https://github.com/QYuQianchen/safe-module-example-faucet)
   * Source code for a tutorial on Safe module creation (also there's a [tweet](https://x.com/QYuQianchen/status/1712079840130793487))    

* [claim settlement](https://github.com/cardstack/safe-module-claim-settlement)
   * This module allows one of a set of addresses (called validators) to sign claims that a caller can use to receive tokens (ERC20 and ERC721) from a safe. Owners of the safe can add and remove validators.
   * Signing claims does not cost any gas, instead the caller must pay for the gas to perform the transfer.
   * Transfers can be conditional on the caller being a specific address, or on the caller holding a specific NFT and they can also be time limited. 

* [safe relay bonded refund module](https://github.com/5afe/safe-relay-bounded-refund-module)
   * SafeRelayBoundedRefund is a module for the Gnosis Safe that relays execTransaction call, a method for executing a transaction in the Gnosis Safe Core contract, and sends gas refund using the chain's native token.  

* [allowance module](https://github.com/BlockchainAsset/allowanceModule)
   * A Safe Module which aids in execution of token transfer via the Safe contract.

* [safe coin](https://github.com/raguiar2/SafeCoin)
   * SafeCoin is a module built on top of the Libray Blockchain the move IR language that grants users a set of capabilities. It also defines a module that acts as a transferrable currency (SafeCoin) and a set of methods through an API that allows a user to access and store SafeCoin. 

* [safe faucet](https://github.com/koshikraj/safefaucet)
   * A module to turn your Safe Accounts into a faucet to drip tokens 

* [safe signature allowance](https://github.com/codebuster22/safe-signature-allowance)
   * A Safe Module contract to allow non-signer accounts to withdraw specified ERC20 tokens to other accounts using safe signer's signature authentication. 

* [safe superuser](https://github.com/dmccartney/safe-superuser)
   * Gnosis Safe module that enables trusted super-users to execute transactions without additional confirmations.   
 
* [safe swap](https://github.com/mattstam/safeswap)
   * A proof-of-concept module that allows token swaps directly from your Safe wallet. 

* [bribefi](https://github.com/lourenc/bribefi)
   * BribeFi is Safe multisig module that allows governance participants to bribe holders to make votes on their behalf. 

* [safe 2 link](https://github.com/koshikraj/safe2link/blob/main/contract/contracts/Safe2LinkModule.sol)
   * Share crypto instantly from your Safe accounts via links

* [farmer safe module](https://github.com/cruzdanilo/farmer-safe-modules) 
* [safe guest module](https://github.com/Alexintosh/Safe-Guest-Module-)
* [safe eip 4337](https://github.com/isabella232/safe-eip4337-module)
* [safe 4337 example](https://github.com/kopy-kat/safe-4337-module-example)
* [cross chain safe](https://github.com/cross-chain-safe/contracts)
 

## Tools

* [SafeScanner](https://www.safescanner.xyz/)
* [create-safe-tx](https://github.com/morpho-labs/create-safe-tx)
* [deploy telor zodiac module](https://github.com/tellor-io/tellor-zodiac-deploy)
* [telor voting ui](https://github.com/tellor-io/votingModule)
* [safe module store](https://github.com/germartinez/safe-module-store)
* [safe street xyz](https://safestreet.xyz/)

## Articles

Blog posts and tutorials related to Safe smart wallets.

* [Safe recovery module](https://dev.to/bxmmm1/safe-recovery-module-1mf)
* [Safe 2 link](https://ethglobal.com/showcase/safe2link-xv25w)
* [Access control management](https://mirror.xyz/finops3.eth/Far9BXCK1V4BPkFhMso9KG-_bbIgnFB0kYdi5-J8Ens)
* [Safe Passkeys: Smooth Onboarding To Every Dapp](https://www.candide.dev/blog/safe-passkeys-smooth-onboarding)

## Projects

Projects using Safe, in alphabetical order

* [Worldcoin](https://github.com/worldcoin)
* [Drakula](https://drakula.app/)
* [Multis](https://multis.com/)
* [Palmera](https://www.palmeradao.xyz/)
* [CirclesUBI](https://joincircles.net/)
* [Den](https://www.onchainden.com/)
* [HQ.xyz](https://www.hq.xyz/)
* [Crypto - the game](https://www.cryptothegame.com/)
* [Olas](https://olas.network/)
* [FluidKey](https://www.fluidkey.com/)
* [NestWallet](https://www.nestwallet.xyz/)
* [Rhinestone](rhinestone.wtf)
* [Zeal](https://www.zeal.app/)
* [Brahma](https://www.brahma.fi/)
* [Candide](https://www.candide.dev/)
* [Karpatkey](https://www.karpatkey.com/)
* [Onit](https://www.onit.fun/)
* [Coinshift](https://coinshift.xyz/)
* [Klaster](https://klaster.io/)
* [Basedapp](https://basedapp.io/)
* [DeFi Saver](https://defisaver.com/)
