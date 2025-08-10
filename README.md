## Download links

- **dlc.dat**：[https://github.com/v2fly/domain-list-community/releases/latest/download/dlc.dat](https://github.com/v2fly/domain-list-community/releases/latest/download/dlc.dat)

## Generate `dlc.dat` manually

## 1. Install the necessary tools

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install git -y
```

```bash
wget https://go.dev/dl/go1.22.6.linux-amd64.tar.gz
sudo tar -C /usr/local -xzf go1.22.6.linux-amd64.tar.gz
```

```bash
echo 'export PATH=/usr/local/go/bin:$PATH' >> ~/.bashrc
source ~/.bashrc
```

## 2. Clone and configure the project

```bash
git clone https://github.com/v2fly/domain-list-community.git
cd domain-list-community
go mod download
```

## 3. Add files to the project

```bash
cd data/
nano win-extra
cd ..
```

## 4. Build a project

```bash
go run ./
```

## 5. Update domains

```bash
cd domain-list-community
nano data/win-extra
go run ./
```
