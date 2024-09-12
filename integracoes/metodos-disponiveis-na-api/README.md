# 🟩 Métodos disponíveis na API

O ArqGED conta com uma lista de métodos disponíveis para uso, dentre estes métodos, temos alguns que já foram reformulados e atualizados para a versão 2.

<table><thead><tr><th width="92">Nº</th><th width="138">Classe</th><th width="354">Método</th><th width="101">Versão</th><th>Status</th></tr></thead><tbody><tr><td>1.1</td><td>Autenticacao</td><td><a href="1.-autenticacao.md#id-1.1-post-api-autenticacao-login">POST/api/Autenticacao/Login</a></td><td>1</td><td></td></tr><tr><td>1.2</td><td>Autenticacao</td><td><a href="1.-autenticacao.md#id-1.2-post-api-autenticacao-refreshtoken">POST/api/Autenticacao/RefreshToken</a></td><td>1</td><td></td></tr><tr><td>2.1</td><td>Arquivo</td><td><a href="2.-arquivo.md#id-2.1-get-api-arquivo-get">GET/api/Arquivo/Get</a></td><td>1</td><td></td></tr><tr><td>2.2</td><td>Arquivo</td><td><a href="2.-arquivo.md#id-2.2-post-api-arquivo-post">POST/api/Arquivo/Post</a></td><td>1</td><td></td></tr><tr><td>2.3</td><td>Arquivo</td><td><a href="2.-arquivo.md#id-2.3-post-api-arquivo-upload">POST/api/Arquivo/Upload</a></td><td>1</td><td></td></tr><tr><td>2.4</td><td>Arquivo</td><td><a href="2.-arquivo.md#id-2.4-delete-api-arquivo-delete">DELETE/api/Arquivo/Delete</a></td><td>1</td><td></td></tr><tr><td>2.5</td><td>Arquivo</td><td><a href="2.-arquivo.md#id-2.5-get-api-arquivo-idimagem-cliente-idcliente">GET/api/Arquivo/{idImagem}/Cliente/{idCliente}</a></td><td>1</td><td></td></tr><tr><td>3.1</td><td>Billing</td><td><a href="3.-billing.md#id-3.1-get-api-billing-get">GET/api/Billing/Get</a></td><td>1</td><td></td></tr><tr><td>3.2</td><td>Billing</td><td><a href="3.-billing.md#id-3.2-get-api-billing-get-conta">GET/api/Billing/Get/Conta</a></td><td>1</td><td></td></tr><tr><td>4.1</td><td>Documento</td><td>PUT/api/Documento/Put</td><td>1</td><td></td></tr><tr><td>4.2</td><td>Documento</td><td>POST/api/Documento/Post</td><td>1</td><td></td></tr><tr><td>4.3</td><td>Documento</td><td>GET/api/Documento/Get</td><td>1</td><td></td></tr><tr><td>4.4</td><td>Documento</td><td>DELETE/api/Documento/Delete</td><td>1</td><td></td></tr><tr><td>5.1</td><td>Lista</td><td>GET/api/Lista/GetListas</td><td>1</td><td></td></tr><tr><td>5.2</td><td>Lista</td><td>GET/api/Lista/GetCamposDaLista</td><td>1</td><td></td></tr><tr><td>5.3</td><td>Lista</td><td>GET/api/Lista/GetLinhaLista</td><td>1</td><td></td></tr><tr><td>5.4</td><td>Lista</td><td>PUT/api/Lista/{idLista}/Cliente/{idCliente}/LinhaLista/{idLinhaLista}</td><td>1</td><td></td></tr><tr><td>5.5</td><td>Lista</td><td>POST/api/AdicionarItemLista/Post</td><td>1</td><td></td></tr><tr><td>5.6</td><td>Lista</td><td>POST/api/Lista/RetornaLinhaListasPorCampoValor/{idLista}/{idUnidade}/{idCliente}</td><td>1</td><td></td></tr><tr><td>6.1</td><td>Workflow</td><td>GET/api/ConfWorkflow/{idCliente}</td><td>1</td><td></td></tr><tr><td>6.2</td><td>Workflow</td><td>POST/api/Workflow/Ativar</td><td>1</td><td></td></tr><tr><td>6.3</td><td>Workflow</td><td>PATCH/api/Workflow/Cliente/{idCliente}/associar-documentos</td><td>1</td><td></td></tr><tr><td>6.4</td><td>Workflow</td><td>GET/api/ConfWorkflow/{idConfWorkflow}/Cliente/{idCliente}/fluxos-ativados</td><td>1</td><td></td></tr><tr><td>6.5</td><td>Workflow</td><td>GET/api/Workflow/Cliente/{idCliente}/dados-fluxo</td><td>1</td><td></td></tr><tr><td>6.6</td><td>Workflow</td><td>GET/api/Workflow/Cliente/{idCliente}/modelo-fluxo</td><td>1</td><td></td></tr><tr><td>6.7</td><td>Workflow</td><td>PATCH/api/Workflow/EtapaExecucao/{IdWorkflowEtapaExecucao}/Cliente/{idCliente}/atualizar-dados-formulário</td><td>1</td><td></td></tr><tr><td>7.1</td><td>Nota Fiscal</td><td>POST/api/NotaFiscal/ImportaNotaFiscal</td><td>1</td><td></td></tr><tr><td>8.1</td><td>Relatórios</td><td>GET/api/Relatorios/GetRelatorios</td><td>1</td><td></td></tr><tr><td>8.2</td><td>Relatórios</td><td>GET/api/Relatorios/GetDadosRelatorios</td><td>1</td><td></td></tr><tr><td>9.1</td><td>Usuário</td><td>POST/api/Usuario/AdicionarUsuario</td><td>1</td><td></td></tr><tr><td>9.2</td><td>Usuário</td><td>PATCH/api/Usuario/{IdUsuario}/AlterarSenhaUsuario</td><td>1</td><td></td></tr><tr><td>9.3</td><td>Usuário</td><td>PATCH/api/Usuario/{IdUsuario}/AlterarStatusUsuario</td><td>1</td><td></td></tr></tbody></table>

***

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
