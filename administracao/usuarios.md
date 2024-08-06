---
description: >-
  No menu Usuários são criados todos os usuários que utilizam o sistema ArqGED e
  atribuídas as permissões de acesso às funcionalidades do sistema.
---

# 🟩 Usuários

## Criando um novo usuário

<figure><img src="../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Empresa:** É apresentado o nome do cliente.

**Adicionar:** Clique para criar um novo usuário.

### **Aba Usuário**

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Nome:** Informe o nome completo do usuário.

**Usuário:** Informe qual será o usuário que deverá ser utilizado na tela de acesso ao sistema.

{% hint style="info" %}
<mark style="color:blue;">Crie um padrão de usuário para sua empresa, como por exemplo: "nome" + "." + "sobrenome" (maria.santos), ou utilize o e-mail corporativo, assim será muito difícil criar um usuário já existente. Quando isso acontece, é apresentada a seguinte mensagem:</mark>

![](<../.gitbook/assets/image (1) (1) (1).png>)

<mark style="color:blue;">Outro ponto importante é que a validação de duplicidade de usuário ocorre em todo o banco de dados do ArqGED e não somente na base utilizada pelo cliente logado no momento.</mark>
{% endhint %}

**Tipo de Acesso:** No caso de usuário de cliente, a única opção disponível é "Cliente".

**Status:** Indica a situação do usuário no sistema. Ao adicionar um novo usuário, será mantido como "**Inativo" até que sejam aplicadas todas as permissões/configurações do usuário.**

**Telefone Fixo e Telefone Celular:** Não são campos de preenchimento obrigatório, porém, estão disponíveis para uso.

**E-mail:** Informe o e-mail mais acessado pelo usuário, este endereço será utilizado para todo o processo de comunicação com o usuário dentro do ArqGED.

**Senha e Confirmar Senha:** Crie uma senha temporária para o usuário considerando os critérios apresentados pelo sistema: _"A senha deve conter no mínimo 8 caracteres, contendo letra maiúscula, minúscula, número e caractere especial."_

**Inativar o usuário depois do dia:** Deve ser utilizado quando o usuário precisar de acesso ao sistema por um determinado período. Ao informar uma data de inativação, automaticamente o usuário será inativado na data previamente cadastrada.&#x20;

**Alterar senha no próximo login:** Marcando o _checkbox_**,** assim que o usuário acessar o sistema pela primeira vez com a senha temporária criada para primeiro acesso, ele deverá criar uma senha pessoal considerando os critérios exigidos pelo sistema.

**Trocar senha a cada \_\_\_ mês:** Marcando o _chackbox_, o sistema deverá de forma automática solicitar o cadastro de uma nova senha, sempre que atingido o prazo estipulado.

**Notificação TTD:** Marcando o _chackbox_, o usuário será notificado quanto ao vencimento dos documentos da sua empresa, caso contratado o serviço.

{% hint style="info" %}
<mark style="color:blue;">É indicada a utilização do</mark> <mark style="color:blue;"></mark>_<mark style="color:blue;">chackbox</mark>_ <mark style="color:blue;"></mark><mark style="color:blue;">"Notificação TTD" apenas para os usuários com permissão de acesso completo a Árvore Documental do cliente, visto que para esta notificação, o sistema não valida o acesso do nível da Árvore Documental sendo o relatório de documentos vencidos enviado na íntegra ao usuário.</mark>
{% endhint %}

### **Aba Permissões I**

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Master:** Informe se o usuário é do tipo Master, ou seja, se ele deve acessar a Árvore Documental completa, sendo necessário neste caso definir somente o perfil de acesso.

Quando é necessária a restrição do usuário por departamento ou tipo documental, ele não poderá ser considerado um usuário Master.

**Clientes que o usuário terá acesso:** Aqui devem ser selecionados todos os clientes que o usuário terá acesso dentro do ArqGED, ou seja, o sistema permite o acesso a vários clientes considerando um login único, ao selecionar o cliente, clique em adicionar "+". Repita o processo até que todos os clientes estejam listados na tela.

Selecione o cliente que deseja definir as permissões para que a Árvore Documental seja habilitada na tela:

<figure><img src="../.gitbook/assets/image (121).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Selecione o perfil que deseja atribuir clicando e arrastando para o nó de Árvore desejado. Para selecionar vários perfis, mantenha o "Ctrl" pressionado e clique nos perfis desejados, arraste os perfis para a Árvore ou clique na opção "Atribuir os perfis selecionados para os níveis de Árvore".

<figure><img src="../.gitbook/assets/image (122).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Clicando no botão de atribuição, será apresentada uma nova tela para indicar em qual nível da Árvore o perfil deve ser aplicado, selecione o desejado e clique "Salvar".

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

{% hint style="warning" %}
<mark style="color:orange;">Se o usuário não for do tipo Master, é possível aplicar permissões diferentes para diferentes nós da Árvore. Se o usuário for do tipo Master, ele terá acesso a toda a Árvore Documental, de acordo com o perfil de acesso definido, por exemplo, se ele tiver perfil de "Edição", ele poderá editar em todos os nós da árvore.</mark>
{% endhint %}

Os perfis são aplicados considerando as atribuições do nível mais alto, então se for arrastado o perfil "pai", todas as permissões "filhas" serão aplicadas ao nó da árvore.

Considerando o exemplo abaixo, ao selecionar o "pai" - Gestão de Documentos para um nó da árvore, automaticamente terá habilitada as permissões filhas:

\- Gestão de Documentos Eletrônicos

&#x20;  \- Eletrônico - Cadastrar, Alterar e Visualizar

&#x20;   \- Eletrônico - Visualizar

&#x20;     \- Eletrônico - Visualizar (não altera)

Caso a restrição precise ser em um nível "filho", é necessário selecionar somente este perfil no momento de arrastar para a árvore, desta forma não serão aplicadas permissões dos níveis superiores ou do nível "pai".

<figure><img src="../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>
