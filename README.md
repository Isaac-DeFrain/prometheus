# prometheus

Prometheus for Mina

Clone the repo, unzip the tar file, copy the config, and run the server

```sh
git clone git@github.com:Isaac-DeFrain/prometheus.git
cd prometheus
tar xvf prometheus-2.43.0.linux-amd64.tar.gz
cp prometheus.yml prometheus-2.43.0.linux-amd64
cd prometheus-2.43.0.linux-amd64
./prometheus --config.file=prometheus.yml
```

Also a good idea, add to `~/.bashrc`

```
alias prometheus="~/prometheus-2.43.0.linux-amd64/prometheus --config=~/prometheus-2.43.0.linux-amd64/prometheus.yml"
```

Use with `mina daemon` options
- `--metrics-port 6060`
- `--libp2p-metrics-port 6061`
