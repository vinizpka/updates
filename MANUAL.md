# Manual do PokePilot

Guia curto do que cada coisa faz. Se você só quer resolver um problema pontual, veja o [FAQ](FAQ.md).

## A barra do topo

| Botão | O que faz |
|---|---|
| **▶ Logar equipe** | Loga de uma vez, com as senhas salvas, as contas que estão fora do jogo. Conta que já está farmando não sai do jogo, a não ser que você tenha trocado o e-mail ou a senha dela no 👤 Treinadores |
| **👤 Treinadores** | Cadastra e-mail e senha de cada conta. O 🗑 limpa o formulário; o 🧹 apaga os dados do jogo daquela conta (resolve conta bugada, a senha continua salva) |
| **⟳ Atualizar tudo** | Recarrega os painéis ligados, ignorando o cache (resolve tela de login velha presa). Pede confirmação: clique de novo em até 4 segundos (com a tecla **R**, aperte duas vezes) |
| **📊 Painel** | A barra lateral com os números de uma conta por vez (detalhes abaixo) |
| **🕹 Cockpit** | Esconde o jogo e mostra só os números das 4 contas. Gasta bem menos do PC |
| **IV's** | Abre a calculadora de IV. Passe o mouse num pokémon dentro do jogo que ela preenche sozinha |
| **🏷 Mercado** | Seus anúncios, vendas e ofertas (Pessoal), o mercado inteiro do jogo com as vendas deduzidas (Global) e a fila de venda (Vender: filtre por raridade, IV, nível, tipo e shiny, marque vários Pokémon, ponha o preço uma vez e anuncie um por um, um clique por anúncio, com a taxa calculada; use com a conta na cidade, o **?** explica por quê) |
| **☰ Opções** | Tudo o mais: Hunt, Quests, Daily, Meta, Boss/Ginásio, Breeding, Scripts, Alertas, Venda protegida, Eco, FAQ... Hunt, Quests e Daily abrem a janela do jogo em todas as contas; se ela já estiver aberta em alguma, fecham em todas |

No cabeçalho de cada painel aparecem selos quando a conta tem **🎁 presente diário** pra pegar ou **📜 quests prontas** pra entregar. Clicar no selo abre a janela só naquela conta.

**Atualização:** a versão nova baixa sozinha em segundo plano e aparece um aviso no canto. Ela só instala quando você clica em **Reiniciar e atualizar**; o app fecha, instala e reabre sozinho. **Depois** guarda o aviso: ele fica ao lado da versão, no topo. Pra procurar na hora, use **☰ Opções > 🔄 Verificar atualização** ou clique na versão do topo: o botão mostra se você já tem a mais nova ou começa a baixar a nova.

**Esc** fecha o card de IV e tira o painel da tela cheia. Com o foco dentro do jogo, aperte **Esc duas vezes** seguidas: um Esc só fica pro jogo (fechar a bolsa, um diálogo) sem mexer no painel.

Atalhos de teclado (só quando o foco está no app, não dentro do jogo, e com nenhuma janela do app aberta): **H** Hunt, **Q** Quests, **D** Daily, **C** Cockpit, **L** Limpar jogo, **R** Atualizar, **T** Treinadores, **G** Meta, **O** Opções, **M** menu do jogo, **E** Eco, **A** Alertas.

## 📊 Painel: a barra lateral

Mostra os números de uma conta por vez. Troque pela aba com o nome da conta no topo do Painel; a aba Σ soma todas.

Na **engrenagem ⚙** do topo dela você escolhe **quais seções aparecem** e arrasta pra reordenar. Duas seções precisam de um passo antes de mostrar algo:

**📌 Itens fixados.** Serve para acompanhar a quantidade de um item específico em todas as contas ao mesmo tempo. Na engrenagem, procure o item (ou a pokébola) pelo nome e clique. Ele passa a aparecer na seção com o total de cada conta. Útil pra bola, revive, pena, o que você estiver juntando.

**🎯 Alvo shiny.** Serve para acompanhar a caçada de um shiny específico. Na engrenagem, em "Alvo shiny", busque a espécie. A seção passa a mostrar se ele **já apareceu**, se foi **capturado** e **quantas bolas** você gastou nele. Sem escolher a espécie, a seção fica vazia explicando isso (antes ela sumia, e parecia que a opção não funcionava).

## 🕹 Cockpit: o painel de todas as contas

O jogo some e ficam só os números das 4 contas. Serve pra deixar farmando gastando pouco do PC. Minimizar ou mandar pra bandeja faz o mesmo com os jogos sozinho, e ao abrir a janela eles voltam. Seções principais:

- **Hoje**: gold, XP, kills e capturas do dia, com meta e o botão que exporta as planilhas
- **Hunts**: o ranking. Ordene por **Sugerido** e escolha o atacante em **"caçar com"**: um Pokémon do time, um do **box** de qualquer conta (grupo "Box · conta") ou **✎ Digitar Pokémon…** (espécie, nível, qualidade e IV; nível da conta e bônus vêm da conta escolhida ao lado). O campo **🔎 hunt ou Pokémon** procura em todas as hunts pelo nome (ex.: venusaur), mesmo as ocultas e fora do escopo escolhido. Golpe de TM só entra na conta se aquele pokémon aprendeu o disco. Com Ditto no time, aparece a melhor transformação por elemento, respeitando o que cada Ditto pode copiar (o Shiny só vira espécie com forma shiny) e sem TM, que Ditto não aprende
  - **🎯 Captura**: cada hunt mostra a chance de capturar por arremesso com a bola escolhida no seletor, quantas bolas custa uma captura (em vermelho quando sai mais caro que o valor de venda) e as capturas/h esperadas. A chance é estimada pela curva do piwtools (valor de venda × eficiência da bola), não é a fórmula do jogo, que roda no servidor. Com o Capture Boost ativo ela dobra. O bônus de rank da profissão não entra. Ao lado aparece a taxa **real** que as suas contas mediram com aquela bola naquela espécie, e esse é o número que vale quando existe
  - **⏳ Respawn e overkill**: nas hunts que você já mediu, a linha mostra a espera por kill fora do combate (andar até o próximo, esperar nascer). Ela muda muito de mapa pra mapa e entra no kills/h e XP/h estimados no lugar do valor único. **⏳ overkill** quer dizer que você mata em ~1 golpe e passa mais tempo esperando o próximo nascer do que batendo: subir de nível não acelera nada ali, e uma hunt mais forte rende mais. O mesmo ⏳ aparece na tabela por conta, ao lado da hunt atual
  - **Aba Hunts**: o ranking ocupa a tela toda, em colunas alinhadas (hunt com nível e região, efetividade, gold/h, XP/h, kills/h e chance de captura), com os seletores numa barra no topo. No **Sugerido** com a Rota de up ligada, a rota aparece numa coluna à direita, como uma linha do tempo: um ponto por faixa de nível, a hunt, do nível tal ao tal, XP/h, tempo e o total embaixo. Na aba **Tudo** a seção continua no formato compacto
  - **🆕 Não capturados**: no filtro de escopo, mostra só as hunts de Pokémon que a conta escolhida ainda não capturou, pela Pokédex do jogo. Em qualquer escopo esses levam o selo 🆕
  - **🏆 Platinar (fila por nível)**: pra completar a Pokédex. Escolha o nível da hunt e aparecem só as espécies dele que a conta ainda não tem, com o progresso (ex.: 14/22). Ao capturar uma espécie nova toca um som e aparece o aviso; **▶ Próxima hunt** (ou **Ir** na linha) abre o Mapa do jogo e clica na hunt por você. O app nunca troca de hunt sozinho: cada viagem é um clique seu (as regras do jogo proíbem ação automática repetida). O apito toca cerca de 1 segundo depois da captura, mesmo com o app escondido ou em outra aba, desde que o escopo Platinar esteja escolhido.
  - **🧭 Rota de up**: no **Sugerido**, marque a caixa e escolha até que nível. O app monta a rota do Pokémon do "caçar com", sem digitar nada: em cada trecho, a hunt de maior XP/h e quanto tempo leva, até o total. A rota corta na dezena (depois 80, 100, 149 e a cada 50), antes de evoluir (com o aviso) e antes de aprender golpe novo. Os stats dos níveis futuros saem da qualidade, do IV e dos TMs reais dele. Por padrão entram as hunts até o nível da conta. Com **só hunts até o nível do Pokémon**, cada trecho fica nas hunts até o nível dele, como no piwtools. As hunts ocultas (✕) ficam de fora. Com o Pokémon de líder há alguns minutos, o tempo usa o XP que ele está ganhando de verdade (VIP e boosts entram aí). Sem essa medição, vale o modelo. Não vale pro Ditto, porque a forma muda a cada hunt
- **Capturas / Shinies**: histórico com filtros por conta, IV, qualidade e período
- **Times & IV**: o time de cada conta com IV, qualidade e poder, e o poder projetado no nível que você escolher (até 3000). Com uns minutos de farm, cada Pokémon que está ganhando XP mostra **⏫ quanto tempo falta pro próximo nível** e **pra evoluir** (ou pro próximo nível redondo), pelo XP/h medido dele. O mesmo aparece no time do painel lateral
- **Inventário**: soma a mochila **e o depósito** das 4 contas
- **Tendência**: gráficos de gold/h e XP/h, e de gold/dia dos últimos 30 dias

## 🏆 Meta (Opções, ou tecla G)

Ranking de todas as espécies base do jogo, todas no nível escolhido (o padrão é o máximo), com IV 32 em cada atributo e qualidade 1,8, a mesma régua do piwdex.com.br/meta. Quatro abas:

- **PvP**: cada espécie luta contra todas as outras. Contra cada rival, cada lado usa o golpe natural que dá mais dano (tabela de tipos do jogo, STAB ×1,5, físico contra Defesa e especial contra Def. Esp., vida = HP × 12) e vence quem precisa de menos golpes pra derrubar o outro; o mesmo número é empate e vale meia vitória. **Vence** é a porcentagem de lutas ganhas; **ataque** é quanto da vida do rival sai por golpe, e **defesa**, quanto da sua sai por golpe recebido (as duas na média contra todos). Lendários lutam como rivais mas ficam fora da lista. Filtre por físicos ou especiais, por tipo (os quadradinhos coloridos) ou busque por Pokémon ou golpe. Clique numa linha pra ver os atributos base, o placar, pra quem ele perde e os golpes com o índice atributo × poder.
- **Hunt**: a hunt que rende mais **gold/h** (ou **XP/h**) pra cada espécie até o nível escolhido, no mesmo modelo do Sugerido do Cockpit (kills/h pelo dano e pelo tempo por golpe calibrado com as suas medições, vezes o loot esperado a preço de NPC). Filtre por Outland ou Orre. O detalhe mostra as 5 melhores hunts, quanto o disco de TM do tipo dele acrescenta e o botão **Ver no Sugerido do Cockpit**.
- **Hunt com TM**: o mesmo, contando o disco elemental do tipo do Pokémon (só estágio final aprende).
- **Seu Pokémon**: escolha um Pokémon do seu time (vem com o nível, a qualidade, o IV e os TMs reais) ou digite qualquer espécie: a lista mostra as melhores hunts pra ele até o nível da conta. Com **Ditto** (comum ou shiny), cada hunt vem com a melhor forma pra virar, respeitando o que o jogo deixa o Ditto copiar.

O botão **Como calculamos** no topo da janela explica tudo isso, e o tier (S, A, B, C, D) vem da posição: 5% S, 15% A, 25% B, 30% C e o resto D. O cálculo roda em pedaços com a janela aberta, sem travar a tela, e fica guardado até os dados do jogo mudarem.

## 🧩 Scripts (Opções)

Userscripts (estilo Tampermonkey) rodando dentro de cada painel do jogo. Marque pra ligar, desmarque pra desligar (desligar recarrega os painéis, e o jogo larga as contas na cidade). Nunca rodam na tela de login.

- **Esconder Pokémon anunciados** (vem com o app, desligado): o jogo mostra no box (breed, transferir, vender) os Pokémon que já estão à venda no mercado. Ligado, eles somem dessas telas. Usa os anúncios da última leitura do **🏷 Mercado**, então precisa de VIP e de a conta ter passado pela cidade. Quando o jogo corrigir, desligue.
- **Os seus**: cole o código, solte um arquivo `.user.js` na janela ou cole o link do arquivo no GitHub. Só instale scripts em que você confia: eles têm acesso total à página do jogo.

## 🥚 Breeding (Opções)

Quantos breeds até a qualidade que você quer e quanto vai custar. Digite a qualidade do Pokémon que vai subir (ex.: 1,274) e a meta (1,7 · 1,8 · 2,0 · 2,5 ou qualquer valor) e clique em **Calcular** (ou Enter); nada recalcula enquanto você digita. A espécie não muda a conta. Cada breed usa o parceiro mais fraco que o jogo aceita (sua qualidade − 0,15): o filho = melhor pai + Δ, então parceiro melhor não ajuda. Com feromônio o Δ é +0,15 (50%), +0,20 (30%), +0,25 (15%) ou +0,30 (5%); no Grátis é uns 20× menor. O filho herda o IV do pai de maior qualidade.

- **Preços**: fee por breed (2 KK), cada stone com quantidade × preço, feromônios por breed × preço e, se você compra os parceiros, o preço de cada um. O preço é seu: o mercado muda. Com o Mercado > Global aberto na sessão aparece a média ao lado, com o botão **usar**. Pokémon de 2 tipos pode pedir 2 stones (**+ stone**).
- **Cotação do jogo**: ao escolher 2 pais no Centro de Breeding do jogo, o app lê a cotação que o jogo mostra (fee, stones, feromônios, teto e chances de Δ) e usa no cálculo. Ele só lê: nunca cria ovo nem pede nada sozinho.
- **Resultado**: uma frase com o normal (breeds, total e tempo chocando), a tabela **Com sorte** (10% melhores), **Normal** e **Com azar** (10% piores) com breeds (= parceiros gastos), fee, stones, feromônios e total, o pior caso possível e o **passo a passo** de uma rodada normal (de quanto pra quanto e a qualidade mínima do parceiro em cada breed). Tempo: 3.000 derrotas por ovo, um de cada vez (o filho é o pai do próximo), pelo kills/h da conta.

## Proteções

- **🛡 Venda protegida**: pede confirmação antes de vender shiny, qualidade Lendária ou acima e itens raros. Na engrenagem do Painel dá pra travar seus próprios itens (**🔒 Cadeado de venda**)
- **🔔 Alertas**: avisa quando aparece shiny, uma conta cai, para de farmar, fica sem suprimento ou tem pokémon derrubado. Na engrenagem do Cockpit você escolhe quais tipos avisam no Windows, um por um. Com webhook do Discord configurado, o aviso também chega no celular
- **⚔️ Luta de boss**: enquanto uma conta luta contra um boss (e até 2 min depois), o aviso de farm parado e o destrava do **↩ Voltar pra hunt** esperam. Mandar a conta de volta pra hunt no meio da luta faria perder a luta
- **💾 Exportar/Importar config**: leva suas configurações e seu histórico pra outro PC. O webhook fica de fora, de propósito. Importar troca o histórico pelo do arquivo e guarda uma cópia do seu antes. O app também salva um backup sozinho toda semana em `%APPDATA%\pokepilot\backups`, a mesma pasta do `hunts-historico.csv` (as hunts que passam das 150 guardadas) e do `hunts-historico-drops.csv`

## Coisas que confundem no começo

- **A opção marcada não mudou nada?** Provavelmente é uma seção que precisa de configuração (Fixados e Alvo shiny). Elas agora dizem isso na tela
- **Os avisos de combate sumiram** ("X derrotado! +XP"): é o **🧼 Limpar jogo**. Desligue-o pra vê-los de novo
- **Não consigo trocar a pokébola**: é o **🧼 Limpar jogo** escondendo o Auto-Helper. Passe o mouse no canto que ele aparece
- **O ouro da sessão**: desde a 1.5.16 vem do próprio servidor do jogo, então é o mesmo número do Hunt Analyzer (menos as Rare Pokemon Picture, se **Considerar preço dos itens no Mercado** estiver marcado, que é o padrão do jogo)
- **Conta travada quando saio do PC**: corrigido na 1.5.16; atualize
