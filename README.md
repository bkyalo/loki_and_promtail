## Installing Loki and Promtail

- Create apt directory

```
mkdir -p /etc/apt/keyrings/
```

- Configure repo source

```
wget -q -O - https://apt.grafana.com/gpg.key | gpg --dearmor > /etc/apt/keyrings/grafana.gpg
```

- Check sources configuration

```
echo "deb [signed-by=/etc/apt/keyrings/grafana.gpg] https://apt.grafana.com stable main" | tee /etc/apt/sources.list.d/grafana.list
```

- Install Loki and Promtal

```
sudo apt install loki promtail
```
