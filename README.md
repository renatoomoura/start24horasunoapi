<p align="center">
	<img src="https://github.com/EngajamentoFlow/unoapi/blob/main/unoapi.png" alt="Quepasa-logo" width="100" />	
	<p align="center">UNOAPI é um software de código aberto, totalmente gratuito, para troca de mensagens com a plataforma Whatsapp</p>
</p>
<hr />
<p align="left">
	<img src="https://telegram.org/favicon.ico" alt="Telegram-logo" width="32" />
	<span>Grupo Telegram: </span>
	<a href="https://t.me/unoapi" target="_blank">Grupo</a>
</p>
<hr />
<p align="left">
	<img src="https://whatsapp.com/favicon.ico" alt="WhatsAPP-logo" width="32" />
	<span>Grupo WhatsaAPP: </span>
	<a href="https://chat.whatsapp.com/KOc9il7AdQVCG06fTmG3Uh" target="_blank">Grupo</a>
</p>
----------------------------------------------------------------------------
</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/liberarunoapi/blob/main/qrcode-pix.png" alt="Quepasa-logo" width="200" />
</p>

**PIX CNPJ**

```
45959142000119	
```

</p>

**Modificação UNOAPI**

Para destravamos 24 horas da UNOAPI, precisamos enviar uma mesagens  como se fosse cliente, "olá" mais essa mensagem não e enviada ou passada para cliente apenas para destravar a tela.
</p>
----------------------------------------------------------------------------
</p>

**Manual de Instalação N8N**

</p>
sudo apt update && sudo apt upgrade
</p>
curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
</p>
sudo apt-get install -y nodejs
</p>
sudo npm install n8n -g
</p>
npm update -g n8n
</p>
npm install pm2 -g
</p>
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
</p>
sudo apt install ./google-chrome-stable_current_amd64.deb
</p>
sudo nano /etc/nginx/sites-available/n8n
</p>

```
server {
  server_name n8n.dominio.com.br;
  location / {
    proxy_pass http://127.0.0.1:5678;
    proxy_http_version 1.1;
    proxy_set_header Upgrade $http_upgrade;
    proxy_set_header Connection 'upgrade';
    proxy_set_header Host $host;
    proxy_set_header X-Real-IP $remote_addr;
    proxy_set_header X-Forwarded-Proto $scheme;
    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
    proxy_cache_bypass $http_upgrade;
    proxy_buffering off;
    proxy_cache off;
  }
  }
```

sudo ln -s /etc/nginx/sites-available/n8n /etc/nginx/sites-enabled
</p>
sudo certbot --nginx
</p>
sudo service nginx restart
</p>
pm2 start n8n --cron-restart="0 0 * * *" -- start
</p>

----------------------------------------------------------------------------

**CONFIGURANDO CERTIFICADO SSL PARA O N8N**

Abra o terminal e execute os seguintes comandos:

cd .n8n/
nano ecosystem.config.js

```
module.exports = {
    apps : [{
        name   : "n8n",
        env: {
            N8N_BASIC_AUTH_ACTIVE:true,
            N8N_BASIC_AUTH_USER:"<usuario>",
            N8N_BASIC_AUTH_PASSWORD:"<sua senha>",
            N8N_PROTOCOL: "https",
            WEBHOOK_TUNNEL_URL: "https://n8n.dominio.com.br/",
            N8N_HOST: "n8n.dominio​.com.br"
        }
    }]
}
```

pm2 start n8n
pm2 start ecosystem.config.js
pm2 startup
pm2 save
</p>

**Acesse ChatWoot**

</p>
Caixas de Entrada
</p>
Adicionar Caixas de Entrada
</p>
Canal do whatsapp
</p>
Nome da Caixa de Entrada (Adicione o que desejar)
</p>
Número de telefone (+Número de telefone)
</p>
ID do número de telefone (+Número de telefone )
</p>
ID da Conta de Negócios (Número de telefone )
</p>
Chave da API (any)
</p>
Print abaixo

<img src="https://github.com/clairton/unoapi-cloud/blob/main/examples/chatwoot/prints/copy_token.png" alt="Quepasa-logo" width="1000" />
<img src="https://github.com/clairton/unoapi-cloud/blob/main/examples/chatwoot/prints/create_channel.png" alt="Quepasa-logo" width="1000" />
<img src="https://github.com/clairton/unoapi-cloud/blob/main/examples/chatwoot/prints/create_contact.png" alt="Quepasa-logo" width="1000" />
<img src="https://github.com/clairton/unoapi-cloud/blob/main/examples/chatwoot/prints/read_qrcode.png" alt="Quepasa-logo" width="1000" />

----------------------------------------------------------------------------
**Agoara vamos prepara modificação Feita**

</p>
Acesse seu N8N baixei Worflow nesse GIT
</p>
Coloque as crediciais do Postgres
</p>
Adionecione uma automação em seu Chatwoot
</p>
COM webhook
</p>
http://localhost:5678/webhook/unoapi
</p>
<img src="https://github.com/EngajamentoFlow/liberarunoapi/blob/main/WhatsApp%20Image%202023-03-23%20at%2012.41.11.jpeg" alt="Quepasa-logo" width="1000" />
</p>
----------------------------------------------------------------------------
----------------------------------------------------------------------------

**Pronto tudo Funcionando**

----------------------------------------------------------------------------
</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/liberarunoapi/blob/main/qrcode-pix.png" alt="Quepasa-logo" width="200" />
</p>

**PIX CNPJ**

```
45959142000119	
```

----------------------------------------------------------------------------
