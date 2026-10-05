# interactor-ecto-bench-tpcc

An order-entry transaction benchmark harness for Elixir that runs against any Ecto adapter.

## What it is for

It supplies the schema, the data loader, the order-entry transactions and a weighted load runner, all adapter-agnostic, so one workload measures whatever repository a caller brings. Its scaling and query design notes are the RFDs in [`rfd`](rfd/).

## Building and running

```sh
mix deps.get
mix test
```

The tests run the workload through `ecto_foundationdb`, so they need that database's client and server installed locally.

## Licence

Apache-2.0. See [LICENSE](LICENSE).
