---
description: >-
  O ArqGED conta com uma lista de métodos disponíveis para uso, na tabela abaixo
  temos o detalhamento de cada um deles.
---

# 🟩 Métodos disponíveis na API

***

<table><thead><tr><th width="76" align="center">Nº</th><th width="95">TAG       </th><th width="162">Método</th><th width="376">Descrição</th><th align="center">Status</th></tr></thead><tbody><tr><td align="center">1.1</td><td>Autenticacao</td><td><mark style="color:blue;"><strong>POST</strong></mark> <a href="1.-autenticacao.md#id-1.1.post-gerar-token-de-autenticacao-v1">/api/Autenticacao/Login</a></td><td> Gerar token de autenticação V1</td><td align="center">Disponível</td></tr><tr><td align="center">1.2</td><td>Autenticacao</td><td><mark style="color:blue;"><strong>POST</strong></mark> <a href="1.-autenticacao.md#id-1.2.post-atualizar-token-de-autenteicacao-v1">/api/Autenticacao/RefreshToken</a></td><td>Atualizar token de autenticação V1</td><td align="center">Disponível</td></tr><tr><td align="center">2.1</td><td>Arquivo</td><td><mark style="color:green;"><strong>GET</strong></mark> <a href="2.-arquivo.md#id-2.1.get-buscar-arquivos-de-um-documento-v1">/api/Arquivo/Get</a></td><td>Buscar arquivos de um documento V1</td><td align="center">Disponível</td></tr><tr><td align="center">2.2</td><td>Arquivo</td><td><mark style="color:blue;"><strong>POST</strong></mark> <a href="2.-arquivo.md#id-2.2.post-cadastrar-arquivos-em-um-documento-v1">/api/Arquivo/Post</a></td><td>Cadastrar arquivos em um documento V1</td><td align="center">Disponível</td></tr><tr><td align="center">2.3</td><td>Arquivo</td><td><mark style="color:blue;"><strong>POST</strong></mark> <a href="2.-arquivo.md#id-2.3.post-cadastrar-arquivos-em-um-documento-retornando-os-ids-das-imagens-v1">/api/Arquivo/Upload</a></td><td>Cadastrar arquivos em um documento, retornando os id's das imagens V1</td><td align="center">Disponível</td></tr><tr><td align="center">2.4</td><td>Arquivo</td><td><mark style="color:red;"><strong>DEL</strong></mark> <a href="2.-arquivo.md#id-2.4.delete-deletar-um-arquivo-de-um-documento-v1">/api/Arquivo/Delete</a></td><td>Deletar um arquivo de um documento V1</td><td align="center">Disponível</td></tr><tr><td align="center">2.5</td><td>Arquivo</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Arquivo/{idImagem}/Cliente/{idCliente}</td><td>Buscar arquivo de um cliente V1</td><td align="center">Disponível</td></tr><tr><td align="center">2.6</td><td>Arquivo</td><td><mark style="color:blue;"><strong>POST</strong></mark> /api/Arquivo/assinar-arquivos</td><td>Assinar eletronicamente arquivos de um Cliente V1</td><td align="center">Disponível</td></tr><tr><td align="center">3.1</td><td>Billing</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Billing/Get</td><td>Buscar as faturas de uma unidade V1</td><td align="center">Disponível</td></tr><tr><td align="center">3.2</td><td>Billing</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Billing/Get/Conta</td><td>Buscar os dados de uma fatura da unidade V1</td><td align="center">Disponível</td></tr><tr><td align="center">4.1</td><td>Documento</td><td><mark style="color:orange;"><strong>PUT</strong></mark> /api/Documento/Put</td><td>Alterar um documento de um Cliente V1</td><td align="center">Disponível</td></tr><tr><td align="center">4.2</td><td>Documento</td><td><mark style="color:blue;"><strong>POST</strong></mark> /api/Documento/Post</td><td>Cadastrar um documento de um Cliente V1</td><td align="center">Disponível</td></tr><tr><td align="center">4.3</td><td>Documento</td><td><mark style="color:blue;"><strong>POST</strong></mark> /api/v2/Documento</td><td>Cadastrar um documento de um Cliente: com compartilhamento V2</td><td align="center">Disponível</td></tr><tr><td align="center">4.4</td><td>Documento</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Documento/Get</td><td>Buscar documentos de um Cliente V1</td><td align="center">Disponível</td></tr><tr><td align="center">4.5</td><td>Documento</td><td><mark style="color:red;"><strong>DEL</strong></mark> /api/Documento/Delete</td><td>Deletar um documento de um Cliente V1</td><td align="center">Disponível</td></tr><tr><td align="center">5.1</td><td>Lista</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Lista/GetListas</td><td>Buscar as listas do Cliente V1</td><td align="center">Disponível</td></tr><tr><td align="center">5.2</td><td>Lista</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Lista/GetCamposDaLista</td><td>Buscar os campos de uma Lista V1</td><td align="center">Disponível</td></tr><tr><td align="center">5.3</td><td>Lista</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Lista/GetLinhaLista</td><td>Buscar os dados de uma Lista V1</td><td align="center">Disponível</td></tr><tr><td align="center">5.4</td><td>Lista</td><td><mark style="color:orange;"><strong>PUT</strong></mark> /api/Lista/{idLista}/Cliente/{idCliente}/LinhaLista/{idLinhaLista}</td><td>Alterar dados de um item de lista V1</td><td align="center">Disponível</td></tr><tr><td align="center">5.5</td><td>Lista</td><td><mark style="color:blue;"><strong>POST</strong></mark> /api/AdicionarItemLista/Post</td><td>Cadastrar um item de lista V1</td><td align="center">Disponível</td></tr><tr><td align="center">5.6</td><td>Lista</td><td><mark style="color:blue;"><strong>POST</strong></mark> /api/Lista/RetornaLinhaListasPorCampoValor/{idLista}/{idUnidade}/{idCliente}</td><td>Buscar itens de lista V1</td><td align="center">Disponível</td></tr><tr><td align="center">6.1</td><td>Workflow</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/ConfWorkflow/{idCliente}</td><td>Buscar configurações de fluxos V1</td><td align="center">Disponível</td></tr><tr><td align="center">6.2</td><td>Workflow</td><td><mark style="color:blue;"><strong>POST</strong></mark> /api/Workflow/Ativar</td><td>Ativar um fluxo V1</td><td align="center">Disponível</td></tr><tr><td align="center">6.3</td><td>Workflow</td><td><strong>PATCH</strong> /api/Workflow/Cliente/{idCliente}/associar-documentos</td><td>Associar documentos a um fluxo V1</td><td align="center">Disponível</td></tr><tr><td align="center">6.4</td><td>Workflow</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/ConfWorkflow/{idConfWorkflow}/Cliente/{idCliente}/fluxos-ativados</td><td>Buscar fluxos ativados de uma configuração V1</td><td align="center">Disponível</td></tr><tr><td align="center">6.5</td><td>Workflow</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Workflow/Cliente/{idCliente}/dados-fluxo</td><td>Buscar dados de um fluxo V1</td><td align="center">Disponível</td></tr><tr><td align="center">6.6</td><td>Workflow</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Workflow/Cliente/{idCliente}/modelo-fluxo</td><td>Buscar modelo de um fluxo V1</td><td align="center">Disponível</td></tr><tr><td align="center">6.7</td><td>Workflow</td><td><strong>PATCH</strong> /api/Workflow/EtapaExecucao/{idWorkflowEtapaExecucao}/Cliente/{idCliente}/atualizar-dados-formulario</td><td>Atualizar formulário de um fluxo V1</td><td align="center">Disponível</td></tr><tr><td align="center">7.1</td><td>Nota Fiscal</td><td><mark style="color:blue;"><strong>POST</strong></mark> /api/NotaFiscal/ImportaNotaFiscal</td><td>Cadastrar nota fiscal como documento: não usar este método. Usar o método POST Documento</td><td align="center">Disponível</td></tr><tr><td align="center">8.1</td><td>Relatórios</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Relatorios/GetRelatorios</td><td>Buscar relatórios V1</td><td align="center">Disponível</td></tr><tr><td align="center">8.2</td><td>Relatórios</td><td><mark style="color:green;"><strong>GET</strong></mark> /api/Relatorios/GetDadosRelatorios</td><td>Buscar dados de um relatório V1</td><td align="center">Disponível</td></tr><tr><td align="center">9.1</td><td>Usuário</td><td><mark style="color:blue;"><strong>POST</strong></mark> /api/Usuario/AdicionarUsuario</td><td>Cadastrar um usuário V1</td><td align="center">Disponível</td></tr><tr><td align="center">9.2</td><td>Usuário</td><td><strong>PATCH</strong> /api/Usuario/{IdUsuario}/AlterarSenhaUsuario</td><td>Alterar senha de um usuário V1</td><td align="center">Disponível</td></tr><tr><td align="center">9.3</td><td>Usuário</td><td><strong>PATCH</strong> /api/Usuario/{IdUsuario}/AlterarStatusUsuario</td><td>Alterar status de um usuário V1</td><td align="center">Disponível</td></tr></tbody></table>

## Códigos Retorno de Validações

### Code: 200 - OK

Este código é a resposta de status de sucesso que indica que a requisição foi bem-sucedida.

### Code: 201 - Created

Este código é retornado quando a requisição foi bem-sucedida e um registro é criado com sucesso.

### Code: 400 - Bad Request

Este erro é retornado quando não for possível interpretar a requisição e/ou o servidor tenta processar a solicitação, mas algum parâmetro da solicitação não é válido, por exemplo, um recurso formatado incorretamente ou uma tentativa de requisição com dados faltantes. As informações sobre a solicitação são fornecidas no corpo da resposta e incluem um código de erro e uma mensagem de erro.

**a-      Item obrigatório**

**b-      Formato incorreto**

**c-       Ids inexistente.**

**d-      Algum parâmetro está incorreto ou é inexistente**

### Code: 401 – Unauthorized

Este erro é retornado quando ocorre alguma falha na autorização e/ou os parâmetros de autenticação estão incorretos.

### Code: 404 Not Found

Este erro é retornado quando o recurso solicitado ou o _endpoint_ não foi localizado.

### Code: 422 - Unprocessable

Este erro é retornado quando a requisição foi recebida com sucesso, porém contém parâmetros inválidos.

### Code: 500  - Server Error

Este erro é retornado quando:

* Ocorre um erro interno no servidor.
* Ocorre uma falha na plataforma ArqGed.
* Formato do parâmetro incorreto.
* Formato do JSON incorreto.

&#x20;
