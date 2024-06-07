# TEMPLATE_UNIFI_CONTROLLER
Template para zabbix Unifi Controller


Template criado com API
Ele mostrará todos os APs do site.

Retornará

Nome do AP;
Modelo do AP;
Tipo do AP;
Versão do AP;
IP do AP;
Estado do AP ( 0 para desligado 1 para ligado);
Se o AP estiver em end of life;
Uptime do AP;

Futuramente podendo adicionar mais itens.

1 - Crie um host por site
2 - No macros do host crie o macro {$UNIFI_SITENAME} e o valor coloque o site_id, que seria o id do site, encontrado na url do controller por exemplo https://192.168.1.10/manage/site/"site_id vai estar aqui"/....
3 - No template aponte os dados do seu controller e crie um usuário de leitura para todos os sites que possuir.
4 - O ip do host é o ip do que será apontado o site, pode colocar o dns ou alterar o script que está no item do template e adicionar o site manualmente, deixando o restante do código intacto funcionará normalmente.

