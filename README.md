# OpenVPN
* Preparando ambiente e configurando servidor de OpenVPN no Ubuntu 20

1° Atualizar o sistema
```
sudo apt update
sudo apt upgrade
```

2° baixar script de instalação
```
wget https://github.com/GeorgeHPD/OpenVPN/blob/bc878fc11a9b87880040e730770ab90301e75971/openvpn-ubuntu-install.sh
```
3° Configurar permissões 
```
chmod -v +x openvpn-ubuntu-install.sh
```
4° Execute o script
```
./openvpn-ubuntu-install.sh
```
5° Siga os passos do script

6° Comandos de Start/Stop/Restart/Status
```
sudo systemctl stop openvpn-server@server.service
sudo systemctl start openvpn-server@server.service
sudo systemctl restart openvpn-server@server.service
sudo systemctl status openvpn-server@server.service
```

7° Execute o script novamente para adcionar novos clientes
```
./openvpn-ubuntu-install.sh
```
