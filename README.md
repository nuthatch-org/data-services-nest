> **Stood down, 13 October 2026.**
>
> Lodestar is offline, and so is everything else I was running for The Graph.
>
> I answered 55 support issues, wrote over 50 forum posts, built and tested over 100 open repos, and helped subgraph devs, indexers and Lodestar users nearly every day. Alone, and unpaid.
>
> Every ask for funding, from a tiny grant ([GIP-0090](https://forum.thegraph.com/t/gip-0090-community-allocation-of-0-1-of-issuance-to-the-nights-watch/7083/2)) to part-time work for the Foundation, was met with hostility. I cant keep going without funding.
>
> To follow my work: [nuthatch-indexer.com](https://nuthatch-indexer.com/)

---

# data-services-nest

A [nuthatch](https://github.com/nuthatch-org/nuthatch) nest of provider registrations on Arbitrum One
for five community Horizon data services: Dispatch, Seahorn, SDSCE, Mainline and the Nuthatch Data
Service. It holds `ProviderRegistered(address,string,string)` and `ProviderDeregistered(address)` and
nothing else, one pair of tables per service (`dispatch__provider_registered`, ...).

Lodestar's service census reads it through kittiwake.

```sh
nuthatch dev --window 25000
```
