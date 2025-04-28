# Instalação VPN Comnect (WNB)

#### 1º Instalar as dependências:  
```bash
apt-get update && apt install bash mawk procps sed grep coreutils net-tools wget cron
```  
_(Vai perguntar se deseja continuar, coloca **S** de sim.)_

#### 2aº Se for pra instalar do zero, usa esse comando: (Instalação)   `./wnbupdate i386 -i`  
_(Se perguntar se deseja update da VPN, coloca **Y** de yes)_     
#### 2bº Se for pra atualizar, usa esse comando: (Atualização)**   `./wnbupdate i386 -u`  
_(Se perguntar se deseja update da VPN, coloca **Y** de yes)_    
 
#### 3aº Checar se o serviço subiu:
```bash
service wnbtlscli status
```  
#### 3b° Se não subir use esse outro:
```bash
service wnbtlscli start
```  
 
#### 4º Sempre ao final da atualização ou instalação do zero da VPN usar o comando abaixo:** 
Esse comando irá garantir que o serviço da VPN sempre inicie com o Linux
```bash
wnbmonitor -r
```

_Reinicie o computador pelo comando `reboot` após rodar os comandos acima._ 
