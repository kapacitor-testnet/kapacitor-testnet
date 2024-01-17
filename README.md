# kapacitor-testnet

Spawning testnets off adjusted filecoin mainnet states to enable advanced testing scenarios in the filecoin ecosystem

## Please note

This is a very early draft of an idea that itself is the cumulation of years of discussions. We allow public access to this document to allow relevant filecoin ecosystem participants to get insight what we are working on and gather some, for now, non public input on the general idea. 

We do not call this a fork as we do not agree with the implications that come with the term itself. Filecoins unique technology allows reusing network states to spawn and maintain networks at very low costs - differentiating filecoin from almost every other blockchain network that exists today. We see clear benefits in exploring this route even with a lot of the underlying thoughts not being laid out publicly at the moment - they will eventually be written down at some point.

As the idea relies heavily on fielcoin miners participating in newly spawned networks they are - for now - the main audience for this document. 

## What now?

We will start a new filecoin network in the coming weeks to explore the details of reusing states to spawn new networks. While we will be able to do this in private at first successive iterations of testing will need support from a broader miner audience. 

Please let us know if you would want to participate in earlier testing of the idea!


## Contact 

Send us a [mail](mailto:kapacitor@factor8.dev) or ping [@f8-ptrk](https://filecoinproject.slack.com/team/U062KS3HPS5) in the filecoin slack for input!

# Summary

The kapacitor testnet is an iterative filecoin testnet spawned off the filecoin mainnet. Utilizing variants of the filecoin mainnets state it will enable more andvanced testing on all levels of the filecoin ecosystem. 



# Motivation

Existing filecoin testnets are focussed on transitioning the filecoin mainnet smoothly between hard forks (network upgrades). With filecoin being a mix of PoW and PoS in combination with its unique storage feature makes testing a challange. By spawning a new testnet off the filecoin mainnets state we currently see 3 main areas of the ecosystem being enabled to do more advanced testing:

## Miners

Testing in the filecoin ecosystem as a miner at scale has always been a struggle. The hardware and logistics a miner needs to properly test beyond a couple of sectors is not insignificant. With no small sector testnet available its costly.

Luckily the nature of PoRep brings it that sectors can be proven on more than a single network. with nothing more than an additional daemon and a prover miners could prove their mainnet sectors on a testnet spawned off the filecoin mainnet state.

## L2 applications

While many applications are deployed on the filecoin L2 testing edge scenarios are almost impossible to test. 

[eg. miner defi failing due to miners failing etc]

## Cryptoeconomic innovation

The fiecoin crypto economics are complex. Attemps to change then, so far, all failed. A lack of a proper test environment played it's role in these failings as simulations only can provide an abstracted picture of the filecoin mainnets reality. Utilizing the mainnets state will allow to peoperly test the impacts of cryptoeconomic changes on the actualk mainnet mechanics. 

# Network outline

This testnet is not meant to be a long running testnet but would be organized in iterations. not all miners will participate, not all miners will choose to maintain their sectors over time - resulting in the testnet degrading and possibly becoming unuseable. 

We currently think iteration cycles of 3 or 6 month would be sufficient to enable the advanced testing imagined. 

With each iteration the adjustments to the mainnet state to spawn off might vary to enable more specific test scenarios as needed.

## Faucet

A testnet without free funds cannot be participated in. To not interupt the economics of the state used to spawn the network off we propose to put vested pre sale funds into the hands of the networks operators to make them available for a faucet

## Notaries / Datacap

To simplify certain iterations of the testnet it might be considered that notaries and non sealed datacap will be removed from a network. 

# Iterations

## Iteration 0 (inception)

the first iteration of the kapacitor testnet will fullfil a few purposes:

- examplify the idea
- develop the tooling needed to repeatedly iterate kapacitor testnets

besides logistical matters we aim to test the following mainnet mechanics on the k0 network:

- burn the mining reserve, a result of https://github.com/filecoin-project/FIPs/discussions/901 



