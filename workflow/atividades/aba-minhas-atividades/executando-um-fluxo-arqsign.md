# ➡️ Executando um fluxo - ArqSign

## Envio dos Documentos para Assinatura via ArqSign <a href="#envio-dos-documentos-para-assinatura-via-arqsign" id="envio-dos-documentos-para-assinatura-via-arqsign"></a>

Quando o fluxo atinge uma etapa do tipo **ArqSign**, a aplicação realiza automaticamente a integração com a plataforma de assinaturas, enviando os documentos que foram **marcados para assinatura**.

Neste momento, é gerada uma **tarefa de acompanhamento** no workflow, destinada aos usuários configurados como **responsáveis pela etapa**. A definição desses responsáveis é feita na aba **Configuração** da própria etapa ArqSign.

## Atividade de Acompanhamento <a href="#atividade-de-acompanhamento" id="atividade-de-acompanhamento"></a>

Enquanto o fluxo ainda **não avança para a próxima etapa**, a tarefa de acompanhamento permanece ativa e acessível para os usuários definidos como **responsáveis pelo acompanhamento** da etapa.

Durante esse período, os usuários podem **monitorar o andamento do processo de assinatura** e, conforme as permissões configuradas na etapa, realizar **ações manuais**, tais como:

* **Cancelar o processo** enviado para o ArqSign;
* **Reenviar o processo**, caso o link de assinatura tenha expirado antes da conclusão;
* **Editar signatários** que ainda não assinaram.

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F2752216790-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fa8U8D6rT1WQEBeHaKsxV%252Fuploads%252FScDuoxgmwIGyoFr54yeM%252Fimage.png%3Falt%3Dmedia%26token%3D653e403f-2dcb-4b7a-b50c-1ae9570b9353&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=1a6812f3&#x26;sv=2" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### **Interação com Token e Signatários**

Na aba **Configurações** da etapa ArqSign, existem dois campos que controlam a possibilidade de interação com processos em andamento:

* **Permitir atualizar token ArqSign expirado**
* **Permitir editar signatários que não assinaram**

As permissões se comportam da seguinte forma:

* **Se ambos os campos estiverem marcados**, o responsável pela tarefa poderá, **em uma única ação**, editar os signatários pendentes e **atualizar o token expirado** dos mesmos, garantindo continuidade ao processo de assinatura.
* **Se apenas o campo “Permitir editar signatários que não assinaram” estiver marcado**, o usuário poderá realizar edições **somente enquanto o processo estiver dentro do prazo de validade**. Caso o token expire, nenhuma ação será possível, a menos que a permissão de atualização também esteja ativada.

### Ação: Cancelar Processo ArqSign <a href="#acao-cancelar-processo-arqsign" id="acao-cancelar-processo-arqsign"></a>

Esta ação estará disponível **somente se** a etapa do tipo ArqSign possuir marcada a configuração **“Permitir cancelar o processo ArqSign”**.

Ao clicar no botão **Cancelar Processo**, o sistema:

* Verifica se todas as obrigatoriedades da tarefa estão preenchidas;
* Exibe uma **mensagem de confirmação** solicitando que o usuário valide a intenção de cancelamento.

Caso o usuário **não confirme**, a mensagem será fechada e a tela da tarefa permanecerá inalterada. Caso o usuário **confirme**, o ArqGED, via integração, realiza o **cancelamento do processo na plataforma ArqSign** e **avança o fluxo conforme o conector configurado para a opção “Cancelado”**.

### Ação: Reenviar Processo ArqSign <a href="#acao-reenviar-processo-arqsign" id="acao-reenviar-processo-arqsign"></a>

O botão **Reenviar Processo** será exibido **somente quando**:

* A etapa do tipo ArqSign possuir a configuração **“Permitir atualizar token ArqSign expirado”**;
* E o processo de assinatura estiver **vencido**.

Se a opção **“Obrigar comentário antes desta ação”** estiver marcada, o sistema irá apresentar uma **tooltip** indicando a obrigatoriedade de comentário, e se ele **já foi registrado ou não**.

Ao acionar esta ação, o sistema exibe a **modal de Reenvio de Processo**, permitindo ao responsável reenviar o processo de assinatura aos signatários com tokens expirados.

### Ação: Editar e Reenviar Processo ArqSign <a href="#acao-editar-e-reenviar-processo-arqsign" id="acao-editar-e-reenviar-processo-arqsign"></a>

O botão **Editar e Reenviar Processo** será exibido **somente se** a etapa possuir a configuração **“Permitir editar signatários que não assinaram”**.

Importante:

* Quando **somente esta opção estiver marcada**, a ação estará disponível **apenas enquanto o processo não estiver vencido**;
* Caso o processo esteja vencido e **não exista permissão para atualização do token**, o botão **não será exibido**.

Se a opção **“Obrigar comentário antes desta ação”** estiver habilitada, o sistema também apresentará uma **tooltip de obrigatoriedade**, informando se já foi preenchida.

Ao clicar nesta ação, o sistema exibirá a **modal “Editar e Reenviar Processo”**, onde será possível ajustar os dados dos signatários que ainda não assinaram e reenviar o processo à plataforma ArqSign.

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F2752216790-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fa8U8D6rT1WQEBeHaKsxV%252Fuploads%252FGPePlAO5KSUxcTG15kX0%252Fimage.png%3Falt%3Dmedia%26token%3Df2105fbb-e86b-45ee-9221-cceaeb20d5e0&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=38da1351&#x26;sv=2" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Ícone: Anexos <a href="#icone-anexos" id="icone-anexos"></a>

O **ícone de Anexos** estará visível na tarefa de acompanhamento e tem o objetivo de exibir todos os documentos envolvidos no processo de assinatura via ArqSign.

Ao acionar o ícone, o sistema **exibe uma modal com os documentos relacionados** à etapa, conforme o tipo e status da tarefa.

#### **Etapas diferentes de ArqSign**

Quando o fluxo possui **etapas comuns com obrigatoriedade de seleção de documentos para assinatura**, esta modal será usada para visualizar, ordenar e confirmar os documentos marcados para envio ao ArqSign.

{% hint style="warning" %}
O sistema **permite selecionar até 25 arquivos** para envio ao ArqSign, somando:

* Anexos do fluxo;
* Anexos dos registros;
* Modelo do fluxo.
{% endhint %}

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F2752216790-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fa8U8D6rT1WQEBeHaKsxV%252Fuploads%252FzFbKmFaZJ4UoZ1mQ0Z2I%252Fimage.png%3Falt%3Dmedia%26token%3Dfc063dbc-ceba-4aa1-9823-6e699711c086&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=4ca92cc&#x26;sv=2" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### **Etapas do tipo ArqSign**

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F2752216790-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fa8U8D6rT1WQEBeHaKsxV%252Fuploads%252FFRHhIgWU7sS20ByCjfN0%252Fimage.png%3Falt%3Dmedia%26token%3Dafefe508-fd59-401e-8d96-b193c7b2c0e6&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=a3681faa&#x26;sv=2" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### **Documentos Assinados**

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F2752216790-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fa8U8D6rT1WQEBeHaKsxV%252Fuploads%252FndAgX4zH6VKxt7NULVNp%252Fimage.png%3Falt%3Dmedia%26token%3D6eb6ebe1-0a7c-44e2-88c2-2e99b1267057&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=3fc78aba&#x26;sv=2" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Ícone: Processo ArqSign <a href="#icone-processo-arqsign" id="icone-processo-arqsign"></a>

O **ícone de Processo ArqSign** permite visualizar informações detalhadas sobre o andamento da etapa de assinatura eletrônica integrada ao fluxo.

**Acompanhamento do Processo**

Ao acionar o ícone, o sistema **exibe uma modal com as informações completas do processo de assinaturas**, permitindo que o usuário acompanhe:

* O **status geral do processo** (em andamento, concluído, cancelado, expirado etc.);
* A **ordem dos signatários** e suas respectivas ações (se já assinaram, recusaram ou estão pendentes);
* A **data e hora de cada movimentação** dentro do processo;
* Quais documentos estão sendo assinados e seu status individual.

Essa modal facilita o acompanhamento técnico do processo e é fundamental para decisões relacionadas ao reenvio, cancelamento ou edição dos signatários, conforme permissões da etapa.

#### **Processo de assinaturas em andamento**

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F2752216790-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fa8U8D6rT1WQEBeHaKsxV%252Fuploads%252FCfe81KSK6x5pBri6GHng%252Fimage.png%3Falt%3Dmedia%26token%3D8fcb02d7-ae9c-44ab-a39b-510dd7ae5a60&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=99bc3426&#x26;sv=2" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

#### **Processo de assinaturas concluído**

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F2752216790-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fa8U8D6rT1WQEBeHaKsxV%252Fuploads%252Fb3M6Dmw8LZgBz1Q0Pw3B%252Fimage.png%3Falt%3Dmedia%26token%3D172b501e-d868-4d90-828e-9d3f61c121f4&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=3e90e56f&#x26;sv=2" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

## Recebimento dos Dados via Webhook ArqSign <a href="#recebimento-dos-dados-via-webhook-arqsign" id="recebimento-dos-dados-via-webhook-arqsign"></a>

Sempre que houver uma interação relevante no processo de assinatura, a plataforma ArqSign envia, via **webhook**, os dados de acompanhamento para o ArqGED. Estes dados são processados automaticamente pelo sistema para garantir o acompanhamento em tempo real por parte dos responsáveis definidos na tarefa.

As situações que disparam o envio de dados via webhook incluem:

✅ Processo assinado por algum signatário;

❌ Processo com falha de envio;

🚫 Processo recusado por algum signatário;

🛑 Processo cancelado pelo remetente;

⏳ Processo expirado.

Ao receber os dados de **conclusão**, o ArqGED realiza o tratamento e avança automaticamente o fluxo com base nas configurações dos **conectores de saída** definidos na etapa do tipo ArqSign. Os possíveis encaminhamentos são:

➡️ Avançar se **Concluído**: Todos os signatários concluíram a assinatura.

➡️ Avançar se **Alguém recusou assinar**: Um ou mais signatários recusaram a assinatura.

➡️ Avançar se **Cancelado**: Processo cancelado no ArqSign ou na tarefa de acompanhamento do ArqGED.

➡️ Avançar se **Link de assinatura expirado**: Opção opcional, ativada apenas se não houver tratamento manual de reenvio na etapa do tipo ArqSign.

## Anexos – Dados da Assinatura <a href="#anexos-dados-da-assinatura" id="anexos-dados-da-assinatura"></a>

Após a conclusão do processo de assinatura, o sistema disponibiliza a visualização e o download do registro de assinaturas vinculadas a cada documento assinado.

Para isso, o usuário deve acionar o **ícone de assinatura** localizado ao lado do nome do arquivo/documento. Ao clicar no ícone, o sistema abre a **modal de assinaturas**, onde é possível:

* Visualizar os dados de cada signatário;
* Consultar data e hora das assinaturas;
* Baixar o **registro completo de assinaturas**.

Essa funcionalidade é essencial para fins de auditoria, comprovação legal e rastreabilidade dos documentos assinados digitalmente via ArqSign.

### Workflow > Atividade > Anexos Visualizar dados de assinaturas <a href="#workflow-greater-than-atividade-greater-than-anexos-visualizar-dados-de-assinaturas" id="workflow-greater-than-atividade-greater-than-anexos-visualizar-dados-de-assinaturas"></a>

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F2752216790-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fa8U8D6rT1WQEBeHaKsxV%252Fuploads%252FF2B6MUSqKDjqyxhrltPg%252Fimage.png%3Falt%3Dmedia%26token%3D3194d44a-5f1c-4ab1-b48e-35bb28a09a37&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=486c47f6&#x26;sv=2" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Visualizar documento > Aba Arquivos <a href="#visualizar-documento-greater-than-aba-arquivos" id="visualizar-documento-greater-than-aba-arquivos"></a>

<figure><img src="https://manual.arquivar.com/~gitbook/image?url=https%3A%2F%2F2752216790-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Fa8U8D6rT1WQEBeHaKsxV%252Fuploads%252Fgw5gh4yEhArkeuGG3ZEQ%252Fimage.png%3Falt%3Dmedia%26token%3D47f433eb-71bc-4bcd-b23a-17cf0b9d8ee7&#x26;width=768&#x26;dpr=4&#x26;quality=100&#x26;sign=4f1e801&#x26;sv=2" alt=""><figcaption><p>Clique na imagem para ampliar.</p></figcaption></figure>

### Baixar Registro de Assinaturas <a href="#baixar-registro-de-assinaturas" id="baixar-registro-de-assinaturas"></a>

Na **modal de dados de assinaturas**, o usuário tem a opção de realizar o download do certificado com o registro de assinaturas do documento.

Para isso, basta acionar o botão <mark style="color:blue;">**\[Baixar Certificado de Assinaturas]**</mark>. Ao clicar, o sistema ArqGED realiza automaticamente o **download do arquivo** contendo o histórico completo das assinaturas realizadas via ArqSign.

Este certificado pode ser utilizado como comprovante legal da integridade e autenticidade das assinaturas digitais realizadas.
