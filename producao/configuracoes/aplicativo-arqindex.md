# 🔹 Aplicativo ArqIndex

O aplicativo ArqIndex é necessário para o trabalho de digitalização e indexação dos documentos, seja na unidade ou no cliente. Este aplicativo deve ser instalado na máquina que será utilizada como servidor, na qual ocorrerão os processos.

## Instalação do aplicativo ArqIndex <a href="#instalacao-do-aplicativo-arqindex" id="instalacao-do-aplicativo-arqindex"></a>

A instalação do ArqIndex no cliente ou em uma das unidades franqueadas deve ser feita pela Arquivar Master mediante solicitação da própria unidade Arquivar franqueada por meio do ArqAtende.

<details>

<summary>Passo a passo para abertura de chamado no ArqAtende</summary>

1. Acesse o site: [https://b24-sd3f59.bitrix24.site/Solicitacoesclientes/](https://b24-sd3f59.bitrix24.site/Solicitacoesclientes/)&#x20;
2. Preencha os campos apresentados na tela:

* _Nome da Empresa_
* _Dados de contato:_ Informe o nome, e-mail e telefone de quem deve receber o retorno do chamado. Essa pessoa precisa ter condições de repassar informações do processo, pois ela poderá ser contata pelos técnicos da Arquivar Master durante a execução do chamado.&#x20;

3. Clique em “Próximo”.
4. No campo “Departamento Atendimento Solicitação” informe o departamento que deve receber sua solicitação.

</details>

***

### Requisitos mínimos <a href="#requisitos-minimos" id="requisitos-minimos"></a>

Alguns processos executados pela aplicação ArqIndex podem demandar um alto processamento de máquina, como memória, processador, espaço em disco, tráfego de rede e internet. É importante que seja avaliado cada detalhe do projeto, pois esta máquina é um grande diferencial, levando em consideração a quantidade de documentos digitalizados bem como a qualidade e tamanho dos arquivos. Seguem os requisitos mínimos da máquina que irá receber a instalação do aplicativo ArqIndex:

* Processador de quatro núcleos;
* 8 GB de memória RAM;
* Espaço de armazenamento em disco de acordo com a demanda de processamento, sendo o mínimo de 250 GB. Caso a unidade ou cliente demande um espaço maior de armazenamento, é recomendável utilizar uma máquina de 500 GB ou mais de armazenamento interno.

***

### Instalação <a href="#instalacao" id="instalacao"></a>

Após de realizar o download do executável de instalação, execute a instalação, selecione o idioma desejado e clique em “OK”. Nas próximas telas, apenas clique em “Próximo” para instalação padrão.

<figure><img src="../../.gitbook/assets/app01.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Por padrão, a pasta de destino da instalação sempre será C:\Program Files (x86)\Arquivar\ArqIndex. O usuário pode escolher outra pasta de destino se desejar.

<figure><img src="../../.gitbook/assets/app02.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Acesso ao ArqIndex <a href="#acesso-ao-arqindex" id="acesso-ao-arqindex"></a>

Depois de instalar o aplicativo do ArqIndex, realize o login utilizando o mesmo usuário e senha de acesso ao ArqGED.

<figure><img src="../../.gitbook/assets/app03.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>



{% hint style="warning" %}
<mark style="color:orange;">**Para acessar o ArqIndex o usuário precisa possuir permissão de acesso ao ArqIndex devidamente habilitada na tela Administração > Usuários > Aba Permissões I > Perfil de acesso: Gestão ArqINDEX. Um usuário pode possuir apenas permissão de indexação, de configuração do local de trabalho ou de correção do XML, ou pode possuir uma permissão global, que permite o acesso a todos os menus.**</mark>
{% endhint %}

***

## Configurar Parâmetros <a href="#configurar-parametros" id="configurar-parametros"></a>

Após o login é exibida a tela de configuração dos parâmetros para o funcionamento da aplicação.

**Local de Trabalho:** Neste campo são exibidos os Parâmetros Gerais ou o chamado Local de Trabalho, criados no menu [Produção > Configurações > Parâmetros Gerais](parametros-gerais.md).

**Local dos Arquivos de Entrada:** Neste campo é informada a pasta onde serão armazenados os arquivos XML e imagens digitalizadas no scanner. É importante que esta pasta esteja compartilhada na rede, pois será utilizada tanto pelo ArqIndex para indexação quanto pelo scanner para digitalização.

**Local dos Arquivos em Processo:** Neste campo é informada a pasta onde serão armazenados os arquivos processados e validados corretamente pelo ArqIndex para indexação. É importante que essa pasta esteja compartilhada na rede, pois será utilizada pelo ArqIndex para indexação dos documentos.

**Local dos Arquivos em Exportação:** Neste campo é informado a pasta onde serão armazenados os arquivos processados, validados e indexados corretamente pelo ArqIndex. É importante que esSa pasta esteja compartilhada na rede, pois será utilizada pelo ArqIndex para exportação dos documentos indexados para o ArqGED.

**HOST/IP:** Este campo é preenchido automaticamente com o endereço da rede onde foi instalada a aplicação ArqIndex.

{% hint style="warning" %}
<mark style="color:orange;">**Após clicar no botão "Salvar" não será mais possível alterar o Local de Trabalho informado, portanto, tenha total certeza de que o endereço informado é o correto.**</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/app05.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Após criadas as pastas para a configuração dos parâmetros, clique sobre cada pasta criada com o botão direito do mouse, selecione Propriedades > Compartilhamento e copie o “Caminho de Rede” conforme o exemplo abaixo. Após copiado, basta colar o caminho no campo correspondente na aplicação ArqIndex. O ideal é que sejam atribuídos às pastas nomes de fácil identificação.

{% hint style="info" %}
<mark style="color:blue;">**EXEMPLO:**</mark>&#x20;

* <mark style="color:blue;">Local dos Arquivos de Entrada: Entrada</mark>
* <mark style="color:blue;">Local dos Arquivos em Processo: Processo</mark>
* <mark style="color:blue;">Local dos Arquivos em Exportação: Exportação</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/app06.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/app07.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

O campo “HOST/IP” é preenchido automaticamente com o endereço de rede onde está instalado o robô do ArqIndex. Clique em “Salvar”.

<figure><img src="../../.gitbook/assets/app08.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

***

## Processos <a href="#processos" id="processos"></a>

Após salvar as configurações, na aba Processos são exibidos as etapas de execução da aplicação, que serão executadas conforme definidas no menu [Produção > Configurações > Fluxo de Trabalho](fluxo-de-trabalho.md).

Inicialmente, sugerimos que seja iniciado o processo de Host das Imagens, clicando-se no ícone “Play”. Quando iniciado, serão criados um certificado para utilização da aplicação ArqIndex na máquina onde foi instalado e outro para ser instalado nas maquinas indexadoras, ou seja, as máquinas onde os usuários irão realizar a indexação dos documentos. Esses certificados são importantes para a comunicação entre a máquina servidor e as máquinas indexadoras.

Os certificados serão criados na pasta onde o aplicativo está instalado (por padrão, na pasta C:\Program Files (x86)\Arquivar\ArqIndex\Certificados).

{% hint style="warning" %}
<mark style="color:orange;">**A máquina de instalação da aplicação ArqIndex precisa ter permissão de Administrador, pois serão criados os certificados automaticamente. Além disso, é necessário:**</mark>

* <mark style="color:orange;">**Liberar a porta 8087 para uso do ArqIndex;**</mark>
* <mark style="color:orange;">**Verificar o firewall, para que não bloqueie o acesso;**</mark>
* <mark style="color:orange;">**Verificar bloqueios de antivírus à aplicação.**</mark>
{% endhint %}

<figure><img src="../../.gitbook/assets/app10.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Será criada uma pasta com os certificados necessários para a indexação dentro do local onde o aplicativo está instalado (por padrão, a pasta C:\Program Files (x86)\Arquivar\ArqIndex).

<figure><img src="../../.gitbook/assets/app09.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Na etapa “Conversão” deve ser definida a quantidade de núcleos do processador que deverão ser dedicados exclusivamente para o processo de conversão dos documentos, que demanda mais recursos da máquina. Depois de realizar essa definição, clique em “Play”.

<figure><img src="../../.gitbook/assets/app11.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

Ao iniciar o processo de indexação, clique em “Play” em “Todos os processos”.

<figure><img src="../../.gitbook/assets/app12.png" alt=""><figcaption><p>Clique para ampliar a imagem.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">**O ideal é que a máquina que for receber o robô do ArqIndex seja dedicada exclusivamente a essa função, já que serão consumidos muito espaço de armazenamento e memória pelo aplicativo e permaneça ligada. Caso seja necessário desligar a máquina ou interromper o ArqIndex por algum motivo, retorne a essa tela e clique em “Pause” em “Todos os processos”.**</mark>
{% endhint %}
