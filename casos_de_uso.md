# **Casos de uso** <h1>

### Nome: <h3>
> Fazer login

### Atores envolvidos: <h3>
> Usuário/gerenciador e sistema

### Fluxo principal: <h3>
> -1.0) [Usuário / Gerenciador] ativa login;
> -2.0) [Usuário / Gerenciador] adiciona email e senha;
> -3.0) [Usuário / Gerenciador] ativa verificação;
> -4.0) [Sistema] valida email e senha;
> -5.0) [Sistema] encerra tela de login.

### Fluxos alternativos: <h3>
## Login usando a conta Google <h2>
> -1.0) [Usuário / Gerenciador] ativa a opção “Entrar com Google” na tela de login.
> -2.0) [Sistema] redireciona o usuário para a página de autenticação do Google.
> -3.0) [Usuário / Gerenciador] insere suas credenciais Google (email e senha).
> -4.0) [Google] valida as credenciais.
> -5.0) [Sistema] recebe do Google os dados de autenticação confirmados (ex.: email, nome).
> -6.0) [Sistema] verifica se já existe conta vinculada a esse email:
>  - Se existir, inicia sessão imediatamente.
>  - Se não existir, cria conta automaticamente com os dados recebidos e inicia sessão.
> -7.0) [Sistema] encerra a tela de login e leva o usuário à tela inicial.

### Pré-condições: <h3>
> O usuário/gerenciador precisa ter uma conta criada

### Pós-condições: <h3>
> O usuário/gerenciador estará logado no sistema e o registro deve ser cadastrado


### Nome: <h3>
> Criar conta

### Atores envolvidos: <h3>
> Usuário e sistema

### Fluxo principal: <h3>
> -1.0) [Usuário] ativa “criar conta”;
> -2.0) [Usuário] adiciona username, email e senha;
> -3.0) [Usuário] ativa verificação;
> -4.0) [Sistema] valida username, email e senha;
> -5.0) [Sistema] leva usuário a tela inicial.

### Fluxos alternativos: <h3>
## Cadastro com dados importados do Google <h2>
> -1.0) [Usuário] ativa “criar conta com Google”;
> -2.0) [Sistema] redireciona para a página de autenticação do Google;
> -3.0) [Usuário] autoriza compartilhamento de dados;
> -4.0) [Sistema] recebe username, email e foto de perfil pré-preenchidos;
> -5.0) [Usuário] confirma ou edita informações;
> -6.0) [Sistema] valida dados e conclui criação de conta;
> -7.0) [Sistema] leva usuário à tela inicial.

### Pré-condições: <h3>
> O usuário ainda não estar logado (sem sessão ativa) e possuir email, username e senha válidos

### Pós-condições: <h3>
> O usuário estará logado no sistema e o registro deve ser cadastrado


### Nome: <h3>
> Adicionar filme/novela/série

### Atores envolvidos: <h3>
> Usuário e sistema

### Fluxo principal: <h3>
> -1.0) [Usuário] acessa a opção “Adicionar novo título”
> -2.0) [Sistema] exibe campo para busca ou cadastro de novo título
> -3.0) [Usuário] seleciona o título e escolhe a lista desejada
> -4.0) [Sistema] confirma a adição à lista

### Fluxos alternativos: <h3>
## Adicionar título diretamente da recomendação do sistema <h2>
> -1.0) [Usuário] acessa a aba “Recomendações”;
> -2.0) [Usuário] escolhe um título sugerido;
> -3.0) [Usuário] seleciona a lista de destino (“Assistido”, “Assistindo” ou “Quero assistir”);
> -4.0) [Sistema] confirma a adição e exibe mensagem de sucesso.

### Pré-condições: <h3>
> O usuário deve estar logado no sistema, deve estar na tela principal, deve ter algum título adicionado em sua lista de “Assistido”, “Assistindo” ou “Quero assistir” e deve estar dentro da página da lista de  “Assistido”, “Assistindo” ou “Quero assistir

### Pós-condições: <h3>
>  O título será adicionado à lista escolhida e ficará disponível para gerenciamento de progresso, avaliação e comentários


### Nome: <h3>
> Buscar por título

### Atores envolvidos: <h3>
> Usuário e sistema

### Fluxo principal: <h3>
> -1.0) [Usuário] acessa a opção de busca
> -2.0) [Sistema] exibe um campo de busca
> -3.0) [Usuário] digita o nome do filme/série ou do diretor
> -4.0) [Usuário] confirma a busca (apertando “Enter” ou clicando em “buscar”)
> -5.0) [Sistema] valida a existência do título
> -6.0) [Sistema] exibe lista de resultados relacionados
> -7.0) [Usuário] pode clicar em um dos itens para ver os detalhes ou adicioná-lo à sua lista

### Fluxos alternativos: <h3>
## Busca por título com autocompletar<h2>
> -1.0) [Usuário] acessa a opção de busca.
> -2.0) [Sistema] exibe o campo de busca.
> -3.0) [Usuário] começa a digitar o nome do filme/série ou do diretor.
> -4.0) [Sistema] exibe sugestões automáticas em tempo real.
> -5.0) [Usuário] seleciona um título diretamente da lista sugerida.
> -6.0) [Sistema] exibe a página de detalhes do título selecionado.

### Pré-condições: <h3>
>  Estar logado no sistema

### Pós-condições: <h3>
>  O sistema apresenta os resultados da busca


### Nome: <h3>
> Visualizar série/filme/novela

### Atores envolvidos: <h3>
> Usuário e sistema

### Fluxo principal: <h3>
> -1.0) [Usuário] acessa a tela de uma de suas listas (“Assistindo”, “Assistido” ou “Quero assistir”).
> -2.0) [Usuário] clica no botão/ícone “Filtro”.
> -3.0) [Sistema] exibe painel de filtros (status, gênero, ano, duração, diretor etc.).
> -4.0) [Usuário] seleciona os critérios desejados e clica em “Aplicar”.
> -5.0) [Sistema] filtra e exibe os títulos que correspondem aos critérios.
> -6.0) [Sistema] atualiza contagem total e exibe resultados filtrados.

### Pré-condições: <h3>
>  O usuário deve ter títulos em sua lista.

### Pós-condições: <h3>
>  O sistema exibe a lista com os filtros aplicado.


### Nome: <h3>
> Cadastrar filme/série/novela

### Atores envolvidos: <h3>
> Gerenciador e sistema

### Fluxo principal: <h3>
> -1.0) [Gerenciador] acessa painel de administração.
> -2.0) [Gerenciador] clica em “Adicionar título”.
> -3.0) [Sistema] exibe formulário com campos: nome, tipo (filme/série/novela), ano, duração, gênero, diretor, elenco, sinopse, capa (upload) e fonte (se TMDb/OMDb etc.).
> -4.0) [Gerenciador] preenche os campos obrigatórios e clica em “Salvar”.
> -5.0) [Sistema] valida campos (sem vazio, formatos corretos).
> -6.0) [Sistema] salva o novo título no catálogo.
> -7.0) [Sistema] exibe confirmação: “Título cadastrado com sucesso.”
> -8.0) [Sistema] exibe o novo título na lista de administração e torna-o pesquisável pelos usuários.

### Pré-condições: <h3>
>  Estar logado no sistema

### Pós-condições: <h3>
>  O título que foi adicionado estará disponível para aos usuários


### Nome: <h3>
> Comentar filme/série/novela

### Atores envolvidos: <h3>
> Usuário e sistema

### Fluxo principal: <h3>
> -1.0) [Usuário] acessa a lista “Assistidos” ou a lista “Assistindo”
> -2.0) [Sistema] exibe os títulos da lista
> -3.0) [Usuário] seleciona um título da lista
> -4.0) [Sistema] exibe detalhes do título, incluindo episódios
> -5.0) [Usuário] seleciona um episódio, capítulo ou seção para comentar
> -6.0) [Sistema] exibe a opção “Adicionar comentário”
> -7.0) [Usuário] clica em “Adicionar comentário”
> -8.0) [Sistema] exibe um campo para digitar o comentário
> -9.0) [Usuário] digita o comentário e clica em “Comentar”
> -10.0) [Sistema] salva o comentário e o exibe vinculado ao título/episódio/capítulo

### Pré-condições: <h3>
>  O título deve estar na lista do usuário. O usuário deve estar logado.

### Pós-condições: <h3>
>   O comentário será salvo e exibido junto ao título correspondente.


### Nome: <h3>
> Avaliar filme/série/novela

### Atores envolvidos: <h3>
> Usuário e sistema

### Fluxo principal: <h3>
> -1.0) [Usuário] acessa a lista “Assistido”
> -2.0) [Usuário] seleciona o título a ser avaliado
> -3.0) [Usuário] escolhe a quantidade de estrelas 
> -4.0) [Usuário] clica em “Salvar avaliação”
> -5.0) [Sistema] salva os dados e exibe a avaliação registrada

### Pré-condições: <h3>
>   O título deve estar marcado como “Assistido”.

### Pós-condições: <h3>
>   A avaliação será salva e poderá ser editada posteriormente.


### Nome: <h3>
> Adicionar resenhas

### Atores envolvidos: <h3>
> Usuário e sistema

### Fluxo principal: <h3>
> -1.0) [Usuário] acessa lista “Assistidos”.
> -2.0) [Usuário] seleciona um título.
> -3.0) [Sistema] exibe detalhes do título e opção “Adicionar resenha”.
> -4.0) [Usuário] clica em “Adicionar resenha”.
> -5.0) [Sistema] exibe editor de texto para resenha (campo multiline).
> -6.0) [Usuário] digita a resenha e clica em “Salvar resenha”.
> -7.0) [Sistema] valida tamanho mínimo (ex: ≥ 50 caracteres).
> -8.0) [Sistema] salva resenha e exibe confirmação: “Resenha adicionada”.
> -9.0) [Sistema] exibe resenha salva na página do título.

### Pré-condições: <h3>
>  Deve estar logado e o usuário deve ter títulos em sua lista.

### Pós-condições: <h3>
>  A resenha estará disponível para auto-avaliação quando o usuário estiver vendo mais informações sobre o título.



