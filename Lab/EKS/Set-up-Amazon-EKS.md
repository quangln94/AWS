# Set Up Amazon EKS

## 1. Chuẩn bị

### 1.1 Cài đặt `kubectl` trên Node Deploy

Download Amazon EKS-vended kubectl binary:
```sh
curl -o kubectl https://amazon-eks.s3.us-west-2.amazonaws.com/1.16.8/2020-04-16/bin/linux/amd64/kubectl
```

### 1.3 Phân quyền
```sh
chmod +x ./kubectl
```

### 1.4 Copy binary to a folder in your PATH. If you have already installed a version of kubectl, then we recommend creating a $HOME/bin/kubectl and ensuring that $HOME/bin comes first in your $PATH.

```sh
mkdir -p $HOME/bin && cp ./kubectl $HOME/bin/kubectl && export PATH=$PATH:$HOME/bin
```
