<p align="center">
  <img width="550" src="https://raw.githubusercontent.com/anudeepND/whitelist/master/images/logo.png">
</p>    
      
## Domínios comuns da white-list para o Pi-Hole.

Uma coleção robusta de sites comumente listados em branco emprestados de várias fontes, incluindo subreddit Pi-Hole, fórum Pi-Hole, repositório github Pi-Hole e muito mais! Adicione esses domínios à sua configuração do Pi-Hole executando um script ou manualmente e torne sua configuração livre de problemas!
 
* * *

### Descrição

***whitelist.txt*** 
Este ficheiro contém domínios que são seguros para colocar na white list, ou seja, não contém quaisquer sites de rastreio ou de publicidade. A adição deste ficheiro resolve muitos problemas, como o histórico de visualização do YouTube, vídeos em sites de notícias e assim por diante...

### COMANDOS

```
pihole -w google.com googleapis.com gstatic.com youtube.com ytimg.com facebook.com fbcdn.net fb.com instagram.com cdninstagram.com whatsapp.com whatsapp.net microsoft.com live.com microsoftonline.com office.com office365.com skype.com onedrive.com twitter.com twimg.com t.co linkedin.com licdn.com tiktok.com tiktokcdn.com reddit.com redd.it pinterest.com pinimg.com snapchat.com sc-cdn.net github.com githubusercontent.com youtube.com googlevideo.com manifest.googlevideo.com facebook.com fbcdn.net fbcdn.com fb.com fbsbx.com facebook.net fb.me instagram.com cdninstagram.com whatsapp.com whatsapp.net api.whatsapp.com graph.facebook.com graph.instagram.com business.facebook.com

wget https://raw.githubusercontent.com/slyfox1186/pihole-regex/main/domains/exact-whitelist.sql -O exact-whitelist.sql
wget https://raw.githubusercontent.com/anudeepND/whitelist/master/domains/whitelist.txt -O whitelist.txt
wget https://raw.githubusercontent.com/nicholasb2101/PiHole/master/Whitelists/Primary%20Whitelist.txt -O primary-whitelist.txt
wget https://raw.githubusercontent.com/TheSmashy/O365Whitlist/main/domains/whitelist.txt -O o365-whitelist.txt
wget https://raw.githubusercontent.com/Levi2288/AdvancedBlockList/main/Lists/whitelist.txt -O advanced-whitelist.txt
wget https://raw.githubusercontent.com/nilsstreedain/pihole-whitelist/main/exact.txt -O exact-whitelist2.txt
wget https://raw.githubusercontent.com/nilsstreedain/pihole-whitelist/main/regex.txt -O regex-whitelist.txt
wget https://raw.githubusercontent.com/agneevX/whitelist/master/whitelist.txt -O agneev-whitelist.txt


for file in whitelist.txt primary-whitelist.txt o365-whitelist.txt advanced-whitelist.txt exact-whitelist2.txt regex-whitelist.txt agneev-whitelist.txt; do
  while read domain; do
    pihole -w $domain
  done < $file
done

pihole -g

sudo systemctl restart pihole-FTL
```



<p align="center">
  <img width="550" src="https://github.com/user-attachments/assets/75a33a48-8711-4715-a6c3-dc5209a4fb9d">
</p>    
      
## Domínios comuns da block-list para o Pi-Hole.

Uma coleção robusta de sites comumente listados em branco emprestados de várias fontes, incluindo subreddit Pi-Hole, fórum Pi-Hole, repositório github Pi-Hole e muito mais! Adicione esses domínios à sua configuração do Pi-Hole executando um script ou manualmente e torne sua configuração livre de problemas!
                
***

### Descrição

***blocklist.txt*** 
Este ficheiro contém domínios que são seguros para colocar na white list, ou seja, não contém quaisquer sites de rastreio ou de publicidade. A adição deste ficheiro resolve muitos problemas, como o histórico de visualização do YouTube, vídeos em sites de notícias e assim por diante...

***

### Principais características:
- Todo o repositório tem curadoria.
- Novos domínios são adicionados com frequência.
- Suporta a instalação do Docker Pi-Hole.
- Vem com um script de shell, ou seja, você pode adicionar todos os domínios automaticamente em um instante.
- Se é um principiante no Pi-Hole, adicionar estes sites resolve muitos problemas.
       


 
