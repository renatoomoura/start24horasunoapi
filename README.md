<p align="center">
	<img src="https://github.com/EngajamentoFlow/unoapi/blob/main/unoapi.png" alt="Quepasa-logo" width="100" />	
	<p align="center">UNOAPI é um software de código aberto, totalmente gratuito, para troca de mensagens com a plataforma Whatsapp</p>
</p>
<hr />
<p align="left">
	<img src="https://telegram.org/favicon.ico" alt="Telegram-logo" width="32" />
	<span>Grupo Telegram: </span>
	<a href="https://t.me/unoapii" target="_blank">Grupo</a>
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

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>

**Manual de Instalação Chatwoot+UNOAPI**

----------------------------------------------------------------------------
**Manual ChatWoot+UNOAPI**

</p>
Vamos precisar de 1 subdomínios
</p>
1º N8N
</p>
----------------------------------------------------------------------------
</p>

Manual de Instalação N8N
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
server {
</p>
  server_name n8n.dominio.com.br;
</p>
  location / {
</p>
    proxy_pass http://127.0.0.1:5678;
</p>
    proxy_http_version 1.1;
</p>
    proxy_set_header Upgrade $http_upgrade;
</p>
    proxy_set_header Connection 'upgrade';
</p>
    proxy_set_header Host $host;
</p>
    proxy_set_header X-Real-IP $remote_addr;
</p>
    proxy_set_header X-Forwarded-Proto $scheme;
</p>
    proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
</p>
    proxy_cache_bypass $http_upgrade;
</p>
    proxy_buffering off;
</p>
    proxy_cache off;
</p>
  }
</p>
  }
</p>
sudo ln -s /etc/nginx/sites-available/n8n /etc/nginx/sites-enabled
</p>
sudo certbot --nginx
</p>
sudo service nginx restart
</p>
pm2 start n8n --cron-restart="0 0 * * *" -- start
</p>

----------------------------------------------------------------------------
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
<img src="https://github.com/clairton/unoapi-cloud/blob/main/examples/chatwoot/prints/copy_token.png" alt="Quepasa-logo" width="1000" />

**Pronto tudo Funcionando**

</p>
----------------------------------------------------------------------------
</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>
----------------------------------------------------------------------------
