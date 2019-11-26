# fc-cluster
fedora coreos iginition

install fcct 

```
# wget https://github.com/coreos/fcct/releases/download/v0.2.0/fcct-x86_64-unknown-linux-gn
# mv fcct-x86_64-unknown-linux-gnu  /usr/local/bin/fcct
# chmod +x /usr/local/bin/fcct
```

install ct

```
# wget https://github.com/coreos/container-linux-config-transpiler/releases/download/v0.9.0/ct-v0.9.0-x86_64-unknown-linux-gnu
# mv ct-v0.9.0-x86_64-unknown-linux-gnu /usr/local/bin/ct
# chmod +x /usr/local/bin/ct
```

## 01_ssh

```
fcct --strict --pretty --input 01_ssh.fcc --output 01_ssh.ign
```

## 02_crio

```
ct --strict --pretty -in-file 02_crio.yaml -out-file  02_crio.ign

```
