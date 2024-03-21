# 🏭 Produção

O menu Produção refere-se ao módulo ArqIndex do ArqGED. Quando os documentos de um cliente são digitalizados, são adicionados a uma fila de trabalho, que posteriormente é acessada pelos operadores do setor de produção da unidade Arquivar que atende a esse cliente para indexação. A indexação é o processo de cadastrar os metadados de identificação de um documento a partir de sua imagem escaneada, e esse processo é feito por meio do menu Produção.&#x20;

{% hint style="info" %}
<mark style="color:blue;">**1º -**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">Os documentos são digitalizados e é gerada a imagem e o arquivo XML de cada. Esses arquivos são armazenados no servidor, em um local de entrada.</mark>    &#x20;

<mark style="color:blue;">**2º -**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">O ArqIndex lê o arquivo XML e envia o documento para a fila de trabalho.</mark> &#x20;

<mark style="color:blue;">**3º -**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">O operador de produção da unidade Arquivar acessa as imagens dos documentos escaneados.</mark> &#x20;

<mark style="color:blue;">**4º -**</mark> <mark style="color:blue;"></mark><mark style="color:blue;">É feito o cadastro das informações de cada um dos documentos no sistema a partir da imagem, ou seja, o operador visualiza a imagem do documento físico para cadastrar os metadados que aquele documento contém, como nome, matrícula, CPF ou CNPJ, entre outros. Também é cadastrado no sistema o código da caixa em que a versão física daquele documento está arquivada.</mark>  &#x20;
{% endhint %}

***

## &#x20;Pré-requisitos para a utilização do ArqIndex&#x20;

1. Serviço ArqIndex no contrato da unidade/cliente, devidamente cadastrado no menu Cliente > Contratos (esse serviço é necessário para que se consiga fazer as configurações necessárias à utilização e acesso do robô responsável pela leitura, gravação e importação do XML). &#x20;
2. Serviço ArqStorage Total ou ArqStorage Ativo no contrato da unidade/cliente, devidamente cadastrado no menu Cliente > Contratos (esse serviço é necessário para que se consiga fazer o processo de exportação dos documentos indexados para o ArqGED).&#x20;
3. Local de trabalho configurado para a unidade ou o cliente. O local de trabalho é onde são configuradas as pastas de entrada, processo e exportação utilizadas pelo ArqIndex e onde são visualizados os logs de indexação, conversão e exportação. Essa configuração é realizada no menu [Produção > Configurações > Parâmetros Gerais](configuracoes/parametros-gerais.md).
4. Fluxo de trabalho criado para a unidade ou cliente, para definir as etapas que o robô deve executar para concluir a indexação. Essa criação é feita no menu [Produção > Configurações > Fluxo de Trabalho.](configuracoes/fluxo-de-trabalho.md)
5. Criação de um usuário cliente ou unidade com a permissão ArqIndex devidamente parametrizada na tela Administração > Usuários > Aba Permissões I > Perfil de acesso: Gestão ArqINDEX.
6. Definição das árvores organizacionais que serão utilizadas com os respectivos campos customizados ou lista que serão digitalizados definidos.
7. Definição dos Ids da Unidade, do Cliente, dos campos customizados e das árvores organizacionais que serão utilizados para indexação.
8. Códigos de caixa já definidos caso sejam indexações de guarda.

{% hint style="warning" %}
<mark style="color:orange;">**Os requisitos para utilização do ArqIndex dependem também do scanner que será utilizado pela unidade ou pelo cliente. É importante lembrar também que o ArqIndex é recomendado para a digitalização de documentos em grande escala. Para digitalizar uma quantidade menor de documentos, o ideal é utilizar o**</mark> [<mark style="color:blue;">**módulo ArqScan**</mark>](../documento/explorar/modulo-arqscan.md)<mark style="color:orange;">**.**</mark>
{% endhint %}

O menu Produção é composto pelos seguintes submenus:

<table data-view="cards"><thead><tr><th align="center"></th></tr></thead><tbody><tr><td align="center"><a href="cadastrar.md"><mark style="color:green;"><strong>Cadastrar</strong></mark></a></td></tr><tr><td align="center"><a href="configuracoes/"><mark style="color:green;"><strong>Configurações</strong></mark></a></td></tr><tr><td align="center"><a href="correcao-do-xml.md"><mark style="color:green;"><strong>Correção do XML</strong></mark></a></td></tr></tbody></table>
