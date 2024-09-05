# apt.dpeckett.dev

## Usage

```shell
curl -fsL https://apt.dpeckett.dev/signing_key.asc | sudo tee /etc/apt/keyrings/apt-pecke-tt-keyring.asc > /dev/null
echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/apt-pecke-tt-keyring.asc] http://apt.dpeckett.dev $(. /etc/os-release && echo $VERSION_CODENAME) stable" | sudo tee /etc/apt/sources.list.d/apt-pecke-tt.list > /dev/null
```