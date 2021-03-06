# Cenários

É uma estratégia reconhecida para compreender as interações entre ambientes e sistemas, assim como elicitar a parte comportamental do software, sua dinâmica e/ou seu fluxo.

Cada cenário geralmente cobre um pequeno número de interações possíveis, e oferecem diversos tipos de informação em diferentes níveis de detalhamento.



## [C1](#c1)

**Realizar cadastro**

|Objetivo  |
 -----------   |
|Permitir que os usuários se cadastrem |
|**Contexto** |
|Local: Tela inicial,clicando no segundo botão para se [cadastrar](../lexicos/#l26-cadastrar) <br>Pré-Condição: Ter instalado o app<br>Pós-Condição: realiza inscrição<br> |
|**Atores**|
|Usuário que deseja ter cadastro no aplicativo|
|**Recursos**|
|Internet, aplicativo, conta de e-mail|
|**Episódios**|
|Usuário deseja reportar seu estado de saúde<br>Usuário navega até a página Home<br>Clica em algum dos botões "[BEM](../lexicos/#l01-bem)" ou "[MAL](../lexicos/#l02-mal)"<br>Se a opção selecionada for [bem](../lexicos/#l01-bem), o aplicativo salva o estado de saúde<br>Se caso for [MAL](../lexicos/#l02-mal), pede mais informações e em seguida, salva as informações<br>|
|**Restrição**|
|possuir um e-mail|
|**Exceção**|
|Estar offline <br> E-mail inválido<br>Aplicativo estar indisponível<br>Senha inválida<br>Conta já existente<br>


## [C2](#c2)

**Fazer login**

|Objetivo  |
 -----------   |
|Fazer [Login](../lexicos/#l27-login) no aplicativo|
|**Contexto** |
|Local: Tela inicial deve clicar no botão login<br>Pré-Condição: Ter o app instalado<br>Pós-Condição: Usuário faz [login](../lexicos/#l27-login) |
|**Atores**|
|Usuário  que deseja fazer [login](../lexicos/#l27-login) e já fez inscrição|
|**Recursos**|
|Internet, aplicativo, e-mail válido, senha válida|
|**Episódios**|
|Usuário clica no botão "[login](../lexicos/#l27-login)" na tela inicial. Em seguida, inserir os dados de [login](../lexicos/#l27-login) <br> estará logado|
|**Restrição**|
|Usuário ter o aplicativo<br> Usuário possuir cadastro|
|**Exceção**|
|Internet cair<br>Usuário esquecer e-mail<br>Usuário esquecer a senha|

## [C3](#c3)

**Reportar estado de saúde**


|Objetivo  |
 -----------   |
|Reporta estado de saúde|
|**Contexto** |
|Local: Tela Home deve clicar no botão "[BEM](../lexicos/#l01-bem)" ou [MAL](../lexicos/#l02-mal)"<br>Pré-Condição: Ter o app instalado<br>Pós-Condição: Usuário registra o estado de saúde |
|**Atores**|
|Usuário que quer reportar o seu estado de saúde|
|**Recursos**|
|Internet, aplicativo|
|**Episódios**|
|Usuário quer reportar o seu estado de saúde abre o aplicativo<br><br> Usuário clica no botão "[BEM](../lexicos/#l01-bem)" é referente ao seu estado de saúde normal. <br> Usuário clica no botão "[MAL](../lexicos/#l02-mal)" na tela home. Em seguida, responde mais perguntas sobre os sintomas. <br> O sistema salva a opção reportarda.|
|**Restrição**|
|Usuário ter o aplicativo instalado.<br> Usuário estar logado|
|**Exceção**|
|Internet cair<br> Usuário ja ter reportado naquele dia <br> Usuário não logado <br> Sistema indisponível|

## [C4](#c4)

**Visualizar mapa**

|Objetivo  |
 -----------   |
|Vizualizar [mapa](../lexicos/#l04-mapa)|
|**Contexto** |
|Local: Aba [mapa](../lexicos/#l04-mapa) no menu inferior<br>Pré-condição: Estar logado no app<br>Pós-condição: Mapa visualizado|
|**Atores**|
|Usuário que deseja saber como está a situação de risco de contágio na região que se encontra|
|**Recursos**|
|Internet<br>Aplicativo<br>Dispositivo móvel com GPS|
|**Episódios**|
|Usuário abre o aplicativo<br>Usuário seleciona [mapa](../lexicos/#l04-mapa) menu inferior<br>Usuário analisa a região<br>Usuário decide quanto cuidado tomar baseado nas marcações do mapa|
|**Restrição**|
|Aplicativo estar instalado<br>Usuário logado|
|**Exceção**|
|Internet não funcionar<br>Servidor indisponível|

## [C5](#c5)

**Visualizar calendário**

|Objetivo  |
 -----------   |
|Visualizar calendário e estatísticas dos relatos|
|**Contexto** |
|Local: Aba [diário](../lexicos/#l03-diario) no menu inferior<br>Pré-condição: Usuário querer saber como está seu histórico de relatos de estado de saúde<br>Pós-condição: Histórico visualizado
Atores|Usuário|
|**Atores**|
|Usuário que deseja vizualizar o histórico e dados dos relatos|
|**Recursos**|
|Aplicativo<br>Internet|
|**Episódios**|
|Usuário entra no aplicativo<br>Usuário seleciona [diário](../lexicos/#l03-diario) no menu inferior<br>Usuário olha quantas vezes ele reportou seus status como [bem](../lexicos/#l01-bem) e [mal](../lexicos/#l02-mal)<br>Usuário navega pelo calendário e vê quais dias ele reportou e quais não<br>Usuário desliza o calendário para o lado e vê as estatísticas dos status|
|**Restrição**|
|Aplicativo instalado<br>Usuário logado|
|**Exceção**|
|Internet não funcionar<br>Servidor indisponível|


## [C6](#c6)

**Editar dados do perfil**

|Objetivo  |
 -----------   |
|Editar dados de algum perfil associado à conta|
|**Contexto** |
|Menu flutuante na home, opção [Editar perfis](../lexicos/#l19-editar-perfis)<br>Pré-condição: Usuário quer modificar informações de algum dos perfis associado à conta<br>Pós-condição: Infomações modificadas|
|**Atores**|
|Usuário que deseja atualizar os dados de cadastro no aplicativo|
|**Recursos**|
|Aplicativo<br>Internet|
|**Episódios**|
|Usuário entra no aplicativo<br>Usuário abre o menu esquerdo da página inicial<br>Usuário seleciona [Editar perfis](../lexicos/#l19-editar-perfis) no menu<br>Usuário seleciona o perfil que deseja editar<br>Usuário faz as modificações e salva|
|**Restrição**|
|Aplicativo instalado<br>Usuário logado|
|**Exceção**|
|Internet não funcionar<br>Servidor indisponível|

## [C7](#c7)

**Visualizar notícias**

|Objetivo  |
 -----------   |
|Visualizar noticias relacionadas ao contexto da Saúde|
|**Contexto** |
|Local:Tela principal na seção “[Notícias](../lexicos/#l18-noticias)”<br>Pré-condição: Acesso a internet , Usuário cadastrado, app instalado<br>Pós-condição: Tela aberta referente a notícias|
|**Atores**|
|Usuários do Guardiões da saúde|
|**Recursos**|
|Conta no Guardiões da Saúde <br>Usuário busca por notícias antigas<br>Acesso a um smartphone|
|**Episódios**|
|Usuário clica na opção de [notícias](../lexicos/#l18-noticias) na tela principal<br>Usuário busca por notícias antigas<br>Usuário clica nas noticias sendo redirecionado na pagina do Twitter referente aos guardiões|
|**Restrição**|
|Aplicativo instalado<br>Usuário logado|
|**Exceção**|
|Internet não funcionar<br>Usuário não cadastrado<br>Email invalido|

## [C8](#c8)

**Visualizar Dicas**

|Objetivo  |
 -----------   |
|Visualizar Dicas relacionadas ao contexto da Saúde|
|**Contexto** |
|Local:Tela principal na seção  “[Dicas](../lexicos/#l05-dicas)”<br>Pré-condicão: Acesso a internet , Usuário cadastrado, app instalado<br>Pós-condição: Tela aberta referente a [Dicas](../lexicos/#l05-dicas)|
|**Atores**|
|Usuários do Guardiões da saúde|
|**Recursos**|
|Conta no Guardiões da Saúde <br>Usuário busca por dicas relacionadas a saúde<br>Acesso a um smartphone|
|**Episódios**|
|Usuário tem a dúvida sobre farmácias, hospitais na região e busca a aba [Dicas](../lexicos/#l05-dicas) para informações.<br>O usuário tem qualquer dúvida relacionada a Covid-19 como uso de máscaras, prevenção, suspeita de infecção, etc, e busca a seção [Dicas](../lexicos/#l05-dicas) do app.<br>Usuário busca por apoio psicológico durante a pandemia e procura ajuda na seção [Dicas](../lexicos/#l05-dicas).<br>Usuário clica nas noticias sendo redirecionado na pagina do Twitter referente aos guardiões.|
|**Restrição**|
|Aplicativo instalado<br>Usuário logado|
|**Exceção**|
|Internet não funcionar<br>Usuário não cadastrado<br>Email invalido|


## Histórico de revisões

Autor | Versão | Data(dd/mm/aaaa) | Descrição 
------|--------|------------------|----------
Wagner Martins | 1.0 | 01/10/2020 | Informações sobre cenários
Lucas Lopes | 2.0 | 08/10/2020 | Cenários: C1,C2 e C3
Wagner Martins | 2.1 | 09/10/2020 | Cenários: C4, C5 e C6
Murilo Schiler | 2.2 | 18/10/2020 | Cenários:c7 e c8
Wagner Martins | 2.3 | 22/11/2020 | Melhorias de acordo com a [verificação](../verificacao-e-validacao/cenarios): Correção dos Atores e linkagem com os léxicos


## Referências

SOMMERVILLE, Ian. **Engenharia de Software**. Pearson Prentice Hall. ed. 9. São Paulo, 2011.
