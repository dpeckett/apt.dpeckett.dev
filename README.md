# apt.pecke.tt

Damian Peckett's personal APT repository.

## Usage

```shell
curl -fsL https://apt.pecke.tt/signing_key.asc | sudo tee /etc/apt/keyrings/apt-pecke-tt-keyring.asc > /dev/null
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/apt-pecke-tt-keyring.asc] http://apt.pecke.tt $(. /etc/os-release && echo $VERSION_CODENAME) stable" | sudo tee /etc/apt/sources.list.d/apt-pecke-tt.list > /dev/null
```