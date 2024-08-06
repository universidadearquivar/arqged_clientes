---
description: >-
  No menu Usuários são criados todos os usuários que utilizam o sistema ArqGED e
  atribuídas as permissões de acesso às funcionalidades do sistema.
---

# 🟩 Usuários

## Criar novo usuário

<figure><img src="../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Empresa:** É apresentado o nome do cliente.

**Adicionar:** Clique para criar um novo usuário.

### **Aba Usuário**

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Nome:** Informe o nome completo do usuário.

**Usuário:** Informe qual será o usuário que deverá ser utilizado na tela de acesso ao sistema.

{% hint style="info" %}
<mark style="color:blue;">Crie um padrão de usuário para sua empresa, como por exemplo: "nome" + "." + "sobrenome" (maria.santos), ou utilize o e-mail corporativo, assim será muito difícil criar um usuário já existente. Quando isso acontece, é apresentada a seguinte mensagem:</mark>

![](<../.gitbook/assets/image (1) (1) (1) (1).png>)

<mark style="color:blue;">Outro ponto importante é que a validação de duplicidade de usuário ocorre em todo o banco de dados do ArqGED e não somente na base utilizada pelo cliente logado no momento.</mark>
{% endhint %}

**Tipo de Acesso:** No caso de usuário de cliente, a única opção disponível é "Cliente".

**Status:** Indica a situação do usuário no sistema. Ao adicionar um novo usuário, será mantido como "**Inativo" até que sejam aplicadas todas as permissões/configurações do usuário.** Ao finalizar todas as configurações, retorne na aba de usuário e altere o status para "ativo", caso contrário, o usuário não conseguirá logar no sistema.

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

<figure><img src="../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Master:** Informe se o usuário é do tipo Master, ou seja, se ele deve acessar a Árvore Documental completa, sendo necessário neste caso definir somente o perfil de acesso.

Quando é necessária a restrição do usuário por departamento ou tipo documental, ele não poderá ser considerado um usuário Master.

**Clientes que o usuário terá acesso:** Aqui devem ser selecionados todos os clientes que o usuário terá acesso dentro do ArqGED, ou seja, o sistema permite o acesso a vários clientes considerando um login único, ao selecionar o cliente, clique em adicionar "+". Repita o processo até que todos os clientes estejam listados na tela.

Selecione o cliente que deseja definir as permissões para que a Árvore Documental seja habilitada na tela:

<figure><img src="../.gitbook/assets/image (121).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Selecione o perfil que deseja atribuir clicando e arrastando para o nó de Árvore desejado. Para selecionar vários perfis, mantenha o "Ctrl" pressionado e clique nos perfis desejados, arraste os perfis para a Árvore ou clique na opção "Atribuir os perfis selecionados para os níveis de Árvore".

<figure><img src="../.gitbook/assets/image (122).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Clicando no botão de atribuição, será apresentada uma nova tela para indicar em qual nível da Árvore o perfil deve ser aplicado, selecione o desejado e clique "Salvar".

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

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

<figure><img src="../.gitbook/assets/image (123).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Como regra, o sistema permite ao perfil que cria novos usuários, definir acessos iguais ao seu ou inferiores, ele também só consegue criar acessos para os mesmos níveis de árvore que ele visualiza.

{% hint style="danger" %}
<mark style="color:red;">Importante ressaltar que a análise das permissões de cada usuário na árvore é de extrema importância para que os perfis sejam aplicados conforme necessidade e não comprometa a saúdo do sistema. Se por ventura esta análise não for feita e o perfil de acesso for aplicado em toda a árvore para todos os usuários, podem ocorrer casos de lentidão desde o momento do login, onde o sistema já inicia a verificação das permissões de acesso, até o momento da consulta de documentos, onde o sistema verifica na solicitação quais dados podem ser apresentados ao usuário logado.</mark>

<mark style="color:red;">Caso identificada a necessidade de acesso a toda a Árvore Documental, a orientação é que o usuário seja criado do tipo "Master".</mark>
{% endhint %}

Para atribuir uma licença de assinatura digital ao usuário, clique no ícone. Na frente do ícone o sistema apresenta a quantidade de licenças utilizadas x a quantidade de licenças contratadas.

<figure><img src="../.gitbook/assets/image (125).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Para desativar a licença, clique novamente no ícone.

<figure><img src="../.gitbook/assets/image (126).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### **Aba Permissões II**

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Endereço Raiz de Armazenamento de Caixas:** Trata-se da lista de endereços utilizada pelo cliente quando realizada a gestão de arquivo interno. Selecione no _checkbox_ somente aqueles que o usuário poderá acessar. Quando não é realizada essa configuração, o usuário não terá a localização física da caixa no busca de documentos e não visualizará o Menu > Caixa ou Pasta > Endereço do Cliente.

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

**Chefe Imediato:** Selecione na lista apresentada o superior do usuário, em caso de utilização do ArqFlow, o chefe imediato poderá visualizar ou executar atividades de seus subordinados, além de ser notificado quanto ao processo.&#x20;

Dentro do arquivo interno, o chefe imediato também poderá cancelar reservas realizadas por seus subordinados.

**Horário de Trabalho:** Selecione na lista o horário de trabalho praticado pelo usuário, quando cadastrado pelo cliente. Este campo é utilizado no ArqFlow para contabilizar o prazo de execução das atividades. Caso o cliente não utilize é só manter o campo sem preenchimento.&#x20;

**Calendário:** Selecione na lista o horário de trabalho praticado pelo usuário, quando cadastrado pelo cliente. Este campo é utilizado no ArqFlow para contabilizar o prazo de execução das atividades. Caso o cliente não utilize é só manter o campo sem preenchimento.

### Aba Perfil

<figure><img src="../.gitbook/assets/image (127).png" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

Nesta aba temos configurações voltadas para o layout do sistema que será apresentado ao usuário.

**Registros por página:** Informe quantos registros o usuário poderá visualizar por página, a sugestão é que sejam definidos no máximo 20.

**Idioma:** Selecione o idioma que será utilizado, podendo ser Português ou Espanhol.

**Foto de Perfil:** Utilize para fazer o upload da foto do usuário.

**Opções de layout:** Selecione na lista qual como deseja que o usuário veja a tela do sistema.

**Cores Padrão:** Deve ser utilizado para definir qual será a cor aplicada na visão do usuário, porém, o usuário só poderá alterar se no cadastro do cliente tiver sido permitida a mudança com a seleção da possibilidade de "Permitir que o usuário altere o layout padrão".

**Alterar Senha:** Utilize para alterar a senha do usuário criado, quando necessário. Preencha com a nova senha e confirme.&#x20;

{% hint style="warning" %}
<mark style="color:orange;">Concluídas todas as configurações para o novo usuário, salve o cadastro, retorne para a "</mark><mark style="color:orange;">**Aba Usuário"**</mark> <mark style="color:orange;"></mark><mark style="color:orange;">e altere o status para "</mark><mark style="color:orange;">**ativo**</mark><mark style="color:orange;">", caso contrário, o usuário não conseguirá logar no sistema.</mark>
{% endhint %}

## Excluir / Inativar / Bloquear Usuário

