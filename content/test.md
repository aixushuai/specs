---
title: Test Page
weight: 1
bookhidden: true

dashboardWeight: 0.2
dashboardState: reliable
dashboardAudit: n/a
---

# Introduction

Filecoin is a distributed storage network based on a blockchain mechanism.
Filecoin _miners_ can elect to provide storage capacity for the network, and thereby
earn units of the Filecoin cryptocurrency (FIL) by periodically producing
cryptographic proofs that certify that they are providing the capacity specified.
In addition, Filecoin enables parties to exchange FIL currency
through transactions recorded in a shared ledger on the Filecoin blockchain.
Rather than using Nakamoto-style proof of work to maintain consensus on the chain, however,
Filecoin uses proof of storage itself: a miner's power in the consensus protocol
is proportional to the amount of storage it provides.

The Filecoin blockchain not only maintains the ledger for FIL transactions and
accounts, but also implements the Filecoin VM, a replicated state machine which executes
a variety of cryptographic contracts and market mechanisms among participants
on the network.
These contracts include _storage deals_, in which clients pay FIL currency to miners
in exchange for storing the specific file data that the clients request.
Via the distributed implementation of the Filecoin VM, storage deals
and other contract mechanisms recorded on the chain continue to be processed
over time, without requiring further interaction from the original parties
(such as the clients who requested the data storage).

## Embeds

### Github master

{{<embed src="https://github.com/filecoin-project/lotus/blob/master/build/bootstrap.go" lang="go" title="Payment Channel Implementation">}}

### Github tag

{{<embed src="https://github.com/filecoin-project/lotus/blob/v0.7.1/build/bootstrap.go" lang="go" title="Payment Channel Implementation">}}

### Github code comments

{{<embed src="https://github.com/filecoin-project/lotus/blob/master/chain/sync.go" lang="go" title="Sync" symbol="Syncer">}}

### Github code small

#### Lorem ipsum

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam sed congue eros, sit amet efficitur turpis. Ut arcu dui, tempor non ex consequat, dictum egestas est. Morbi et pulvinar magna. Nam scelerisque fermentum felis ut vehicula. Fusce malesuada tortor sed arcu pretium laoreet. Praesent ac nibh eu leo euismod condimentum. Suspendisse vitae fringilla nulla. Donec in fermentum odio. Nullam ut congue leo. Fusce urna lorem, tincidunt ac porta nec, dapibus ac ipsum. Nulla posuere vulputate nisi. Integer eget elementum diam. Aenean tincidunt lectus eu quam tincidunt aliquam. Curabitur eget lacinia diam.

{{<embed src="https://github.com/filecoin-project/lotus/blob/master/chain/sync.go" lang="go" title="Sync" symbol="InformNewHead">}}

### Local file

{{<embed src="test-embed.js" lang="js" title="Test embed JS">}}

## Diagrams

![Protocol Overview Diagram](/intro/diagrams/orient/filecoin.dot)

## Blockquotes

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam sed congue eros, sit amet efficitur turpis. Ut arcu dui, tempor non ex consequat, dictum egestas est.

> **Note**  
> Morbi et pulvinar magna. Nam scelerisque fermentum felis ut vehicula. Fusce malesuada tortor sed arcu pretium laoreet. Praesent ac nibh eu leo euismod condimentum. Suspendisse vitae fringilla nulla. Donec in fermentum odio. Nullam ut congue leo. Fusce urna lorem, tincidunt ac porta nec, dapibus ac ipsum. Nulla posuere vulputate nisi. Integer eget elementum diam. Aenean tincidunt lectus eu quam tincidunt aliquam. Curabitur eget lacinia diam.

## Katex shortcode

Filecoin Miners must commit resources in order to participate in the economy; the protocol can use the minersʼ stake in the network to ensure that rational behavior benefits the network, rewarding the creation of value and penalizing malicious behavior via slashing. The pledge size is meant to adequately incentivize the fulfillment of a sectorʼs promised lifetime and provide sufficient consensus security.

Hence, the {{<katex>}}$sectorQuality = avgQuality*size${{</katex>}}initial pledge function consists of two components: a _storage pledge_ and a _consensus pledge_.

{{<katex>}}

$SectorInitialPledge = SectorInitialStoragePledge + SectorInitialConsensusPledge$

{{</katex>}}

Morbi et pulvinar magna. Nam scelerisque fermentum felis ut vehicula. Fusce malesuada tortor sed arcu pretium laoreet. Praesent ac nibh eu leo euismod condimentum. Suspendisse vitae fringilla nulla. Donec in fermentum odio. Nullam ut congue leo. Fusce urna lorem, tincidunt ac porta nec, dapibus ac ipsum. Nulla posuere vulputate nisi. Integer eget elementum diam. Aenean tincidunt lectus eu quam tincidunt aliquam. Curabitur eget lacinia diam.

{{<katex>}}

$SectorInitialConsensusPledge =  30\% \times FILCirculatingSupply \times \frac{SectorQAP}{max(NetworkBaseline, NetworkQAP)}$

{{</katex>}}

Morbi et pulvinar magna. Nam scelerisque fermentum felis ut vehicula. Fusce malesuada tortor sed arcu pretium laoreet. Praesent ac nibh eu leo euismod condimentum. Suspendisse vitae fringilla nulla. Donec in fermentum odio. Nullam ut congue leo. Fusce urna lorem, tincidunt ac porta nec, dapibus ac ipsum. Nulla posuere vulputate nisi. Integer eget elementum diam. Aenean tincidunt lectus eu quam tincidunt aliquam. Curabitur eget lacinia diam.

{{<katex>}}
$SectorQualityMultiplier = \frac{\sum\nolimits_{deals} DealWeight * DealQualityMultiplier}{SectorSpaceTime}$
{{</katex>}}
