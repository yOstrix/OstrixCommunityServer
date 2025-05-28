## Detalhamento de Tarefas por Sistema

### 1. Sistema de Progressão (Plugin Principal: MMOCore)

**Tarefas Comuns de Configuração:**

*   **Instalação e Configuração Inicial:**
    *   Instalar MMOCore e sua dependência (MythicLib).
    *   Configurar conexão com banco de dados (se aplicável, para maior performance/escalabilidade).
    *   Ajustar configurações globais básicas (experiência, level cap inicial, etc.).
*   **Classes:**
    *   Definir as classes principais do servidor (Guerreiro, Mago, Arqueiro, etc.).
    *   Configurar atributos base para cada classe (força, inteligência, vida, mana, etc.).
    *   Configurar ganho de atributos por nível para cada classe.
    *   Definir skills iniciais de cada classe.
    *   Configurar permissões de acesso às classes (se necessário).
    *   Criar árvores de subclasses ou especializações (se solicitado).
*   **Atributos:**
    *   Revisar e customizar os atributos padrão do MMOCore (Attack Damage, Max Health, etc.).
    *   Criar novos atributos customizados (Resistência Mágica, Chance de Esquiva, etc.), se necessário.
    *   Definir como os atributos escalam e interagem.
*   **Skills/Habilidades:**
    *   Configurar as skills para cada classe (dano, cooldown, custo de mana/stamina, efeitos, etc.).
    *   Criar skills customizadas (pode exigir conhecimento de MythicMobs ou scripting).
    *   Configurar a árvore de skills (skill tree) e pontos de skill por nível.
    *   Definir pré-requisitos para aprender skills (nível, outras skills, classe).
*   **Sistema de Mana/Stamina/Recursos:**
    *   Configurar a regeneração de mana/stamina.
    *   Ajustar os custos de recursos das skills.
    *   Integrar com MMOItems para custos de mana em itens (se aplicável).
*   **Experiência e Níveis:**
    *   Ajustar a curva de experiência (XP necessário por nível).
    *   Configurar fontes de XP (matar mobs, completar quests, profissões, etc.).
    *   Integrar com outros plugins para fontes de XP adicionais (se necessário).
*   **Parties/Grupos:**
    *   Configurar o sistema de parties do MMOCore (tamanho máximo, regras de loot, compartilhamento de XP).
*   **Placeholders e GUI:**
    *   Configurar placeholders do MMOCore para exibição em scoreboards, chat, etc. (requer PlaceholderAPI).
    *   Customizar GUIs internas do MMOCore (árvore de skills, perfil do jogador), se necessário.
*   **Testes e Balanceamento:**
    *   Testar todas as classes, skills e progressão.
    *   Ajustar valores para balanceamento inicial.

**Estimativa de Tempo (Exemplo - Adapte à sua realidade):**
*   Configuração básica: 2-4 horas
*   Configuração por Classe (incluindo skills básicas): 3-6 horas *por classe*
*   Criação de Skills Customizadas: 1-3 horas *por skill* (depende da complexidade)
*   Balanceamento inicial: 5-10 horas

*(Continue para o próximo sistema...)*



### 2. Sistema de Trabalhos (Plugin Principal: MMOCore ou Jobs Reborn)

**Opção A: Usando Profissões do MMOCore**

*   **Configuração:**
    *   Ativar e configurar o módulo de profissões do MMOCore.
    *   Definir as profissões disponíveis (Minerador, Lenhador, Pescador, Alquimista, etc.).
    *   Configurar as fontes de experiência para cada profissão (quebrar blocos específicos, craftar itens, etc.).
    *   Definir os níveis máximos e a curva de experiência para as profissões.
    *   Configurar recompensas por nível de profissão (novas receitas, acesso a áreas, permissões, atributos bônus - pode requerer integração manual ou scripts).
    *   Integrar com outros sistemas (ex: receitas de forja do MMOItems/ItemsAdder que exigem nível de profissão).
*   **Testes:**
    *   Testar o ganho de XP e progressão em todas as profissões.
    *   Verificar se as recompensas e integrações funcionam.

**Opção B: Usando Jobs Reborn (Gratuito)**

*   **Instalação e Configuração Inicial:**
    *   Instalar Jobs Reborn e suas dependências (ex: CMILib, PlaceholderAPI).
    *   Configurar as opções globais do plugin.
*   **Definição dos Trabalhos:**
    *   Criar e configurar cada trabalho (Minerador, Lenhador, Construtor, Caçador, Fazendeiro, etc.).
    *   Definir as ações que dão experiência e dinheiro para cada trabalho (quebrar blocos, matar mobs, pescar, craftar, etc.).
    *   Ajustar os valores de pagamento e experiência por ação.
    *   Configurar os níveis máximos e a curva de experiência para cada trabalho.
    *   Definir limites de quantos trabalhos um jogador pode ter simultaneamente.
*   **Integração e Placeholders:**
    *   Configurar placeholders para exibir informações dos trabalhos (nível, XP, etc.).
    *   Integrar com sistema de economia (Vault).
*   **Testes:**
    *   Testar a progressão, pagamentos e ganho de XP em todos os trabalhos.

**Estimativa de Tempo (Exemplo):**
*   Configuração MMOCore Profissões: 4-8 horas (depende da complexidade e integrações)
*   Configuração Jobs Reborn (por trabalho): 1-3 horas *por trabalho*

### 3. Sistema de Bebidas (Plugin Principal: BreweryX)

**Tarefas Comuns de Configuração:**

*   **Instalação e Configuração Inicial:**
    *   Instalar BreweryX.
    *   Configurar opções básicas (idioma, etc.).
*   **Criação de Receitas:**
    *   Definir as receitas das bebidas (ingredientes, processo de fermentação/destilação).
    *   Configurar o tempo de preparo e dificuldade.
    *   Criar bebidas customizadas com nomes, descrições e efeitos (efeitos de poção, comandos executados, etc.).
    *   Definir a qualidade das bebidas e como ela afeta os efeitos/preço.
*   **Processos (Fermentação, Destilação, Envelhecimento):**
    *   Configurar os blocos necessários para cada processo (caldeirão, alambique, barris).
    *   Ajustar o tempo necessário para cada etapa.
    *   Configurar o envelhecimento em barris (tipos de madeira, tempo, melhoria na qualidade).
*   **Efeitos e Embriaguez:**
    *   Configurar os níveis de embriaguez e seus efeitos (náusea, lentidão, força, mensagens no chat, etc.).
    *   Definir como a embriaguez diminui com o tempo.
*   **Integração:**
    *   Integrar com sistema de economia (Vault) se quiser vender/comprar bebidas.
    *   Integrar com ItemsAdder/MMOItems se quiser usar itens customizados como ingredientes ou as próprias bebidas.
*   **Testes:**
    *   Testar todas as receitas e processos.
    *   Verificar os efeitos das bebidas e o sistema de embriaguez.

**Estimativa de Tempo (Exemplo):**
*   Configuração básica + 5-10 receitas: 3-6 horas
*   Criação de Receitas Complexas Adicionais: 0.5-1 hora *por receita*

*(Continue para o próximo sistema...)*



### 4. Sistema de Tabelionato (Local de Pesquisas)

**Funcionalidade:** Aprendizado de habilidades/magias, obtenção de informações, registro de ID/assuntos jurídicos.
**Plugins Envolvidos:** MMOCore (Skills), Citizens (NPCs), potencialmente plugins de GUI/Comandos Customizados.

**Tarefas Comuns de Configuração:**

*   **NPCs (Citizens):**
    *   Instalar Citizens.
    *   Criar os NPCs que representarão o tabelionato (Tabelião, Instrutor de Magia, Arquivista, etc.).
    *   Configurar a aparência e comportamento básico dos NPCs (skins, poses, falas básicas).
*   **Aprendizado de Habilidades/Magias (MMOCore):**
    *   Integrar NPCs do Citizens com o sistema de skills do MMOCore (ex: NPC que abre a GUI de skills ou ensina skills específicas mediante custo/requisito).
    *   Configurar quais skills podem ser aprendidas no tabelionato e sob quais condições (nível, classe, custo em dinheiro/itens).
*   **Obtenção de Informações:**
    *   Configurar NPCs para fornecerem informações através de diálogos (usando Citizens ou addons como Denizen/BetonQuest).
    *   Criar menus de GUI (usando plugins como DeluxeMenus/ChestCommands - gratuitos) acessíveis via NPC para apresentar informações/lore/tutoriais.
*   **Registro de ID/Assuntos Jurídicos:**
    *   **Solução Simples:** Criar comandos customizados (usando MyCommand/CustomCommands - gratuitos) que simulem um registro (ex: `/registrarid`, que talvez adicione uma permissão ou tag ao jogador via LuckPerms).
    *   **Solução Intermediária:** Usar um plugin de notas ou gerenciamento de dados simples (ex: PlayerNotes - gratuito) para que um "Tabelião" (staff ou NPC com permissões) possa registrar informações sobre jogadores.
    *   **Solução Complexa:** Desenvolvimento de um plugin customizado simples para essa funcionalidade específica (fora do escopo de configuração padrão).
*   **Testes:**
    *   Testar a interação com todos os NPCs.
    *   Verificar o aprendizado de skills e obtenção de informações.
    *   Testar o sistema de registro implementado.

**Estimativa de Tempo (Exemplo):**
*   Configuração NPCs (Citizens básico): 1-2 horas
*   Integração MMOCore Skills com NPC: 1-3 horas
*   Criação de Menus de Informação (GUI): 2-5 horas (depende da quantidade)
*   Configuração Registro Simples (Comandos): 1-2 horas

### 5. Sistema de Comidas (Plugins Principais: ItemsAdder / MMOItems)

**Tarefas Comuns de Configuração:**

*   **Instalação e Configuração Inicial:**
    *   Instalar ItemsAdder ou MMOItems (e dependências como MythicLib para MMOItems).
    *   Configurar o resource pack automático (ItemsAdder) ou manual.
*   **Criação de Comidas/Bebidas Customizadas:**
    *   Definir os itens base (materiais vanilla).
    *   Criar as texturas/modelos para as comidas/bebidas customizadas (pode exigir trabalho de design gráfico ou aquisição de packs prontos).
    *   Configurar os atributos dos itens no plugin (nome, lore, textura, efeitos ao consumir).
    *   Definir efeitos de poção, duração, saturação, fome restaurada.
    *   Criar efeitos customizados (executar comandos, dar buffs temporários específicos do MMOCore, etc.).
*   **Receitas (se aplicável):**
    *   Integrar com o sistema de crafting/forja (ver seção Forja) para permitir que jogadores criem essas comidas/bebidas.
*   **Integração:**
    *   Garantir que as comidas funcionem com sistemas de fome e saturação vanilla ou modificados.
    *   Integrar com lojas ou drops de mobs, se necessário.
*   **Testes:**
    *   Testar a criação (se houver receitas) e o consumo de todas as comidas/bebidas customizadas.
    *   Verificar se os efeitos aplicados estão corretos.

**Estimativa de Tempo (Exemplo):**
*   Configuração básica do plugin: 1-3 horas
*   Criação por Item Customizado (sem textura): 0.5-1 hora *por item*
*   Criação/Adaptação de Textura/Modelo: Varia muito (pode ser rápido com packs prontos ou demorado se for design do zero).

*(Continue para o próximo sistema...)*



### 6. Sistema de Forja (Plugins Principais: MMOItems / ItemsAdder)

**Tarefas Comuns de Configuração:**

*   **Instalação e Configuração Inicial:**
    *   Garantir que MMOItems/ItemsAdder e dependências (MythicLib) estejam instalados e configurados (incluindo resource pack).
*   **Estações de Crafting (Crafting Stations):**
    *   Definir os tipos de estações de forja (Forja de Armas, Forja de Armaduras, Bancada de Alquimia, etc.).
    *   Configurar a aparência das estações (bloco vanilla, bloco customizado do ItemsAdder/MMOItems).
    *   Definir como os jogadores acessam as estações (clique direito no bloco, comando).
*   **Criação de Receitas Customizadas:**
    *   Definir as receitas para cada item a ser forjado (armas, armaduras, ferramentas, consumíveis, etc.).
    *   Especificar os ingredientes necessários (itens vanilla, itens customizados de MMOItems/ItemsAdder).
    *   Configurar as condições para usar a receita (nível do jogador, classe MMOCore, profissão MMOCore, permissão LuckPerms).
    *   Definir o item resultante (item vanilla, item customizado MMOItems/ItemsAdder).
    *   Configurar o tempo de crafting (se aplicável).
    *   Configurar receitas de upgrade/reparo (MMOItems).
*   **Integração:**
    *   Integrar com o sistema de profissões (MMOCore/Jobs) para desbloquear receitas.
    *   Garantir que os itens criados funcionem corretamente com outros sistemas (MMOCore, MMOItems stats, etc.).
*   **Testes:**
    *   Testar todas as estações de crafting e receitas.
    *   Verificar se as condições e ingredientes funcionam.
    *   Confirmar que os itens resultantes são os esperados.

**Estimativa de Tempo (Exemplo):**
*   Configuração básica das estações: 2-4 horas
*   Criação por Receita Customizada: 0.5-1.5 horas *por receita* (depende da complexidade e condições)

### 7. Sistema de Hierarquia (Plugins: LuckPerms, EssentialsXChat, potencialmente MMOCore/FactionsUUID)

**Tarefas Comuns de Configuração:**

*   **Instalação e Configuração Inicial:**
    *   Instalar LuckPerms e EssentialsX (incluindo EssentialsXChat).
    *   Configurar o armazenamento de dados do LuckPerms (arquivo local ou banco de dados).
*   **Grupos de Permissões (LuckPerms):**
    *   Definir a estrutura de ranks/grupos (Membro, VIP, Moderador, Admin, etc.).
    *   Configurar a herança entre os grupos.
    *   Atribuir permissões a cada grupo (comandos vanilla, comandos de plugins, acesso a funcionalidades).
    *   Definir prefixos e sufixos para cada grupo (para exibição no chat).
    *   Configurar tracks de promoção (se o cliente quiser um sistema de /rankup).
*   **Formato do Chat (EssentialsXChat):**
    *   Configurar o formato do chat para exibir os prefixos/sufixos definidos no LuckPerms, nome do jogador, e a mensagem.
    *   Customizar cores e formatação.
*   **Guildas/Facções (Opcional - MMOCore/FactionsUUID):**
    *   Se usar MMOCore Parties: Configurar limites e funcionalidades.
    *   Se usar FactionsUUID (ou similar): Instalar e configurar o plugin de facções (criação, poder, territórios, relações, etc.) - *Esta é uma configuração complexa por si só.*
*   **Testes:**
    *   Testar as permissões de cada grupo.
    *   Verificar a exibição correta de prefixos/sufixos no chat.
    *   Testar o sistema de promoção (se houver).
    *   Testar o sistema de guildas/facções (se implementado).

**Estimativa de Tempo (Exemplo):**
*   Configuração LuckPerms (5-10 grupos básicos): 3-6 horas
*   Configuração EssentialsXChat: 0.5-1 hora
*   Configuração FactionsUUID (básica): 5-10 horas (pode ser muito mais dependendo da customização)

*(Continue para o próximo sistema...)*



### 8. Sistema de Rankings (Plugins: MMOCore, PlaceholderAPI, ajLeaderboards)

**Tarefas Comuns de Configuração:**

*   **Instalação e Configuração Inicial:**
    *   Instalar PlaceholderAPI e ajLeaderboards (ou outra alternativa como LeaderHeads se preferir/adquirir).
    *   Garantir que MMOCore esteja configurado para registrar as estatísticas relevantes (nível, stats, etc.).
    *   Baixar as expansões necessárias do PlaceholderAPI (`/papi ecloud download ...`).
*   **Configuração dos Leaderboards (ajLeaderboards):**
    *   Definir quais estatísticas terão leaderboards (Top Nível, Top Dano, Top Riqueza, etc.).
    *   Configurar os placeholders que serão usados para cada leaderboard (ex: `%mmocore_level%`, `%vault_eco_balance%`, estatísticas de outros plugins).
    *   Customizar a aparência dos leaderboards (formato, número de entradas, atualização).
    *   Configurar como os leaderboards serão exibidos (comandos, NPCs clicáveis, Hologramas - requer HolographicDisplays/DecentHolograms).
*   **Integração MMOCore:**
    *   Verificar se as estatísticas do MMOCore estão sendo corretamente lidas pelo PlaceholderAPI para uso nos leaderboards.
*   **Testes:**
    *   Verificar se os leaderboards atualizam corretamente.
    *   Confirmar se os dados exibidos estão corretos.
    *   Testar os métodos de exibição (comandos, NPCs, hologramas).

**Estimativa de Tempo (Exemplo):**
*   Instalação e configuração básica PAPI/ajLeaderboards: 1-2 horas
*   Configuração por Leaderboard: 0.5-1 hora *por leaderboard*
*   Configuração de exibição (Hologramas/NPCs): 1-3 horas

### 9. Sistema de Comercio (Plugins: EssentialsX, QuickShop Reremake, AuctionHouse)

**Tarefas Comuns de Configuração:**

*   **Instalação e Configuração Inicial:**
    *   Instalar EssentialsX, QuickShop Reremake, AuctionHouse (versão gratuita) e Vault (dependência essencial para economia).
    *   Configurar um plugin de economia compatível com Vault (ex: EssentialsX Eco, CMI Eco, ou outro).
*   **Trocas (EssentialsX):**
    *   Geralmente funciona por padrão com `/trade`. Verificar permissões se necessário.
*   **Lojas de Jogadores (QuickShop Reremake):**
    *   Configurar opções gerais (limite de lojas por jogador, itens proibidos, logs, etc.).
    *   Ajustar a aparência das lojas (formato das mensagens, display items).
    *   Definir taxas (se houver) para criar lojas.
    *   Configurar permissões de uso (criar, comprar, vender).
*   **Casa de Leilões (AuctionHouse):**
    *   Configurar opções gerais (duração dos leilões, número de itens por página, taxa para listar, itens proibidos, etc.).
    *   Customizar mensagens e interface gráfica (GUI).
    *   Configurar permissões (listar, dar lances, comprar).
    *   Integrar com a economia (Vault).
*   **Testes:**
    *   Testar o comando `/trade`.
    *   Testar a criação, compra e venda em lojas QuickShop.
    *   Testar a listagem, lances e compra na AuctionHouse.
    *   Verificar se o dinheiro está sendo corretamente debitado/creditado (Vault).

**Estimativa de Tempo (Exemplo):**
*   Configuração básica dos plugins + Vault + Economia: 2-4 horas
*   Configuração detalhada QuickShop: 1-2 horas
*   Configuração detalhada AuctionHouse: 2-3 horas