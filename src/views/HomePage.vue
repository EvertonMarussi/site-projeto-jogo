<template>
<div class="home-page-root">
  <section class="hero-section">
    <div class="video-container">
      <video autoplay muted loop playsinline class="bg-video">
        <source src="@/assets/videoHome.mp4" type="video/mp4" />
      </video>
      <div class="overlay-gradient"></div>
    </div>

    <div class="hero-content poppins-regular">
      <div class="text-wrapper">
        <h1 class="hero-title poppins">
          Recupere o reino invadido e <span class="gradient-text">salve e princesa</span> 
        </h1>
        <p class="hero-description">
          A princesa foi sequestrada e o reino foi invadido. Sua missão é combater monstros, matar o rei e recuperar a princesa
        </p>

        <div class="cta-group">
          <button ref="btn1" class="btn-primary poppins-semibold" @click="scrollTo('jogo')">
            CONFERIR JOGO
          </button>
          <button ref="btn2" class="btn-outline poppins-semibold" @click="scrollTo('sobre')">
            SAIBA MAIS
          </button>
        </div>
      </div>
    </div>

    <div class="scroll-indicator" @click="scrollTo('next')">
      <span class="material-symbols-outlined">expand_more</span>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════
       SEÇÃO MOTIVAÇÃO
  ═══════════════════════════════════════════════════ -->
  <section class="section-motivacao" id="motivacao">
    <div class="section-bg-particles" id="motivacao-particles"></div>
    <div class="container">
      <div class="section-header" data-animate="fade-up">
        <span class="section-label">Por que criamos isso</span>
        <h2 class="section-title poppins">Nossa <span class="gradient-text">Motivação</span></h2>
        <p class="section-subtitle">Quatro estudantes, uma missão: transformar uma história épica em uma experiência interativa inesquecível.</p>
      </div>

      <div class="motivacao-grid">
        <div class="motivacao-card" data-animate="fade-up" data-delay="0">
          <div class="card-icon-wrapper">
            <span class="material-symbols-outlined card-icon">sports_esports</span>
            <div class="icon-glow"></div>
          </div>
          <h3 class="card-title poppins-semibold">Paixão por Jogos</h3>
          <p class="card-text">Crescemos jogando e sonhando em criar. Este projeto nasceu do desejo genuíno de construir algo que nos representa — um jogo com alma, lore profundo e mecânicas que desafiam o jogador.</p>
          <div class="card-tag">Game Design</div>
        </div>

        <div class="motivacao-card card-featured" data-animate="fade-up" data-delay="150">
          <div class="card-icon-wrapper">
            <span class="material-symbols-outlined card-icon">auto_stories</span>
            <div class="icon-glow green"></div>
          </div>
          <h3 class="card-title poppins-semibold">Narrativa como Motor</h3>
          <p class="card-text">Acreditamos que um bom jogo precisa de uma história que justifique cada batalha. O camponês não é apenas um herói genérico — ele é um homem apaixonado que enfrenta um sistema de poder corrompido por energias sombrias.</p>
          <div class="card-tag featured">Storytelling</div>
        </div>

        <div class="motivacao-card" data-animate="fade-up" data-delay="300">
          <div class="card-icon-wrapper">
            <span class="material-symbols-outlined card-icon">biotech</span>
            <div class="icon-glow"></div>
          </div>
          <h3 class="card-title poppins-semibold">Aprendizado Técnico</h3>
          <p class="card-text">Este projeto é nosso laboratório. Cada sistema de combate, cada animação e cada inimigo foi uma oportunidade de aprender desenvolvimento de jogos na prática, saindo da teoria para o código real.</p>
          <div class="card-tag">Engenharia</div>
        </div>

        <div class="motivacao-card" data-animate="fade-up" data-delay="100">
          <div class="card-icon-wrapper">
            <span class="material-symbols-outlined card-icon">group</span>
            <div class="icon-glow"></div>
          </div>
          <h3 class="card-title poppins-semibold">Trabalho em Equipe</h3>
          <p class="card-text">Quatro mentes, quatro perspectivas e um objetivo comum. Descobrimos como dividir responsabilidades, unificar visões estéticas e criar algo que nenhum de nós conseguiria sozinho.</p>
          <div class="card-tag">Colaboração</div>
        </div>

        <div class="motivacao-card" data-animate="fade-up" data-delay="250">
          <div class="card-icon-wrapper">
            <span class="material-symbols-outlined card-icon">emoji_events</span>
            <div class="icon-glow"></div>
          </div>
          <h3 class="card-title poppins-semibold">Desafiar o Convencional</h3>
          <p class="card-text">Queríamos subverter o RPG clássico. A gosma verde, os mortos vivos, os lobos corrompidos — tudo foi pensado para criar um universo com regras próprias, onde a ciência sombria do rei molda a realidade do jogo.</p>
          <div class="card-tag">Inovação</div>
        </div>

        <div class="motivacao-card" data-animate="fade-up" data-delay="400">
          <div class="card-icon-wrapper">
            <span class="material-symbols-outlined card-icon">palette</span>
            <div class="icon-glow"></div>
          </div>
          <h3 class="card-title poppins-semibold">Arte com Propósito</h3>
          <p class="card-text">Cada cor no jogo conta uma história. O verde corrupto da gosma, o roxo sagrado da floresta, o preto da armadura evoluída — a paleta visual foi projetada para reforçar o lore sem uma única linha de texto.</p>
          <div class="card-tag">Arte Visual</div>
        </div>
      </div>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════
       SEÇÃO HISTÓRIA — MÚLTIPLOS CAPÍTULOS
  ═══════════════════════════════════════════════════ -->
  <section class="section-historia" id="historia">

    <!-- Capítulo 1: O Amor Proibido -->
    <div class="historia-chapter chapter-amor" data-chapter="1">
      <div class="chapter-bg-overlay"></div>
      <div class="chapter-content container">
        <div class="chapter-eyebrow" data-animate="fade-right">
          <span class="chapter-number">01</span>
          <span class="chapter-label">Prólogo</span>
        </div>
        <h2 class="chapter-title poppins" data-animate="fade-right">
          O Amor que <span class="gradient-text">Desafia Fronteiras</span>
        </h2>
        <div class="chapter-body" data-animate="fade-right">
          <p>Nas terras do reino, onde campos férteis se estendem até onde a vista alcança, vivia um camponês sem nome de família, sem brasão, sem título. Mas tinha algo que muitos nobres jamais possuíram: as mãos calejadas de quem realmente constrói o mundo.</p>
          <p>Ele era conhecido em cada aldeia, em cada rua do mercado, em cada colheita. Um homem que ajudava todos, esperava nada em troca, e carregava nos olhos uma chama que poucos conseguiam decifrar.</p>
          <p>A princesa o conheceu pela primeira vez quando ele reparou a roda quebrada de uma carruagem real que havia estacionado no caminho. Sem hesitar, sem pedir permissão, sem esperar recompensa — ele simplesmente resolveu. E foi naquele ato humilde e decisivo que ela o viu de verdade.</p>
        </div>
        <div class="chapter-quote" data-animate="fade-up">
          <blockquote>"Ela estava disposta a não ser mais princesa, caso esse fosse o destino, pois amava mais ao camponês do que todas as riquezas do reino."</blockquote>
        </div>
      </div>
      <div class="chapter-visual chapter-visual-1">
        <div class="visual-card" data-animate="fade-left">
          <span class="material-symbols-outlined visual-icon">favorite</span>
          <span class="visual-label">Um amor impossível</span>
        </div>
      </div>
    </div>

    <!-- Capítulo 2: O Convite -->
    <div class="historia-chapter chapter-convite" data-chapter="2">
      <div class="chapter-bg-overlay dark"></div>
      <div class="chapter-content container reverse">
        <div class="chapter-visual chapter-visual-2">
          <div class="lore-cards-stack" data-animate="fade-right">
            <div class="lore-mini-card">
              <span class="material-symbols-outlined">castle</span>
              <span>O Castelo da Princesa</span>
            </div>
            <div class="lore-mini-card active">
              <span class="material-symbols-outlined">local_cafe</span>
              <span>O Convite ao Café</span>
            </div>
            <div class="lore-mini-card">
              <span class="material-symbols-outlined">diamond</span>
              <span>O Pedido de Mão</span>
            </div>
          </div>
        </div>
        <div class="chapter-text-block">
          <div class="chapter-eyebrow" data-animate="fade-left">
            <span class="chapter-number">02</span>
            <span class="chapter-label">O Encontro</span>
          </div>
          <h2 class="chapter-title poppins" data-animate="fade-left">
            Um Café que <span class="gradient-text">Mudaria Tudo</span>
          </h2>
          <div class="chapter-body" data-animate="fade-left">
            <p>Um dia, contra todos os protocolos da corte, a princesa enviou um convite. Não para um baile de gala, não para uma cerimônia oficial — mas para um simples café no castelo. Uma mensagem singela que carregava um peso enorme.</p>
            <p>O camponês se preparou como nunca havia se preparado para nada. Lavou as roupas, poliu as botas, e guardou algo consigo — um anel talhado à mão, com uma pedra verde encontrada nas margens do rio. Ele pediria sua mão. Sem riquezas, sem título, apenas com a promessa de uma vida inteira de dedicação.</p>
            <p>A princesa estava pronta para dizer sim. Para abrir mão da coroa se necessário. Para escolher o homem que a enxergava como pessoa, não como troféu.</p>
          </div>
        </div>
      </div>
    </div>

    <!-- Capítulo 3: A Invasão -->
    <div class="historia-chapter chapter-invasao" data-chapter="3">
      <div class="chapter-bg-overlay red"></div>
      <div class="chapter-content container">
        <div class="chapter-eyebrow" data-animate="fade-right">
          <span class="chapter-number">03</span>
          <span class="chapter-label">A Tragédia</span>
        </div>
        <h2 class="chapter-title poppins" data-animate="fade-right">
          O Dia que o <span class="gradient-text-red">Reino Caiu</span>
        </h2>
        <div class="chapter-body" data-animate="fade-right">
          <p>O chefe do reino inimigo observava há anos. Invejoso, consumido por uma obsessão que crescia junto com seu poder. Ele não queria o ouro, não queria as terras — ele queria a princesa. E quando soube do convite ao camponês, algo quebrou dentro dele.</p>
          <p>Suas tropas marcharam ao cair da noite. Cavaleiros reais com armaduras que emanavam energia verde e roxa varreram a guarda do palácio. Esqueletos reanimados pela gosma verde do rei encheram as ruas. Os lobos da floresta sagrada — corrompidos, de olhos verdes em vez de roxos — avançaram pelas muralhas.</p>
          <p>O camponês lutou. Com as mãos que eram de construir, não de matar, ele enfrentou o que pôde. Mas o exército do rei era numeroso demais. Ele foi expulso. O reino foi tomado. E a princesa... foi levada.</p>
        </div>
        <div class="invasion-stats" data-animate="fade-up">
          <div class="stat-item">
            <span class="stat-icon material-symbols-outlined">skull</span>
            <span class="stat-value">+4.000</span>
            <span class="stat-label">Inimigos eliminados pelo Cavaleiro Negro</span>
          </div>
          <div class="stat-item">
            <span class="stat-icon material-symbols-outlined">castle</span>
            <span class="stat-value">1</span>
            <span class="stat-label">Reino invadido e tomado</span>
          </div>
          <div class="stat-item">
            <span class="stat-icon material-symbols-outlined">science</span>
            <span class="stat-value">3</span>
            <span class="stat-label">Tipos de energia corrompida</span>
          </div>
          <div class="stat-item">
            <span class="stat-icon material-symbols-outlined">science</span>
            <span class="stat-value">3</span>
            <span class="stat-label">Tipos de energia corrompida</span>
          </div>
        </div>
      </div>
    </div>

    <!-- Capítulo 4: O Lore dos Inimigos -->
    <div class="historia-chapter chapter-lore" data-chapter="4">
      <div class="chapter-bg-overlay deep"></div>
      <div class="container">
        <div class="chapter-eyebrow center" data-animate="fade-up">
          <span class="chapter-number">04</span>
          <span class="chapter-label">O Bestiário</span>
        </div>
        <h2 class="chapter-title poppins center" data-animate="fade-up">
          As Forças da <span class="gradient-text">Escuridão</span>
        </h2>
        <p class="chapter-subtitle" data-animate="fade-up">O rei não apenas conquistou com espadas — ele corrompeu, reanimou e transformou. Cada inimigo é uma vítima de seus experimentos com a gosma verde e a energia roxa roubada da floresta sagrada.</p>

        <div class="bestiary-grid">
          <div class="bestiary-card" data-animate="fade-up" data-delay="0">
            <div class="bestiary-header skeleton-header">
              <span class="material-symbols-outlined bestiary-icon">skull</span>
              <div class="bestiary-rank">
                <span class="rank-dot"></span><span class="rank-dot"></span><span class="rank-dot empty"></span><span class="rank-dot empty"></span><span class="rank-dot empty"></span>
              </div>
            </div>
            <h3 class="bestiary-name poppins-semibold">Esqueletos</h3>
            <p class="bestiary-lore">Soldados caídos de guerras passadas — tanto aliados quanto inimigos do rei. Seus corpos foram mergulhados no líquido verde e reanimados como servos sem vontade. Frágeis individualmente, devastadores em hordas.</p>
            <div class="bestiary-tags">
              <span class="tag">Reanimado</span>
              <span class="tag">Baixa resistência</span>
              <span class="tag">Alta quantidade</span>
            </div>
          </div>

          <div class="bestiary-card" data-animate="fade-up" data-delay="100">
            <div class="bestiary-header knight-header">
              <span class="material-symbols-outlined bestiary-icon">shield</span>
              <div class="bestiary-rank">
                <span class="rank-dot"></span><span class="rank-dot"></span><span class="rank-dot"></span><span class="rank-dot empty"></span><span class="rank-dot empty"></span>
              </div>
            </div>
            <h3 class="bestiary-name poppins-semibold">Cavaleiros Reais</h3>
            <p class="bestiary-lore">Guerreiros de elite reequipados com armas que canalizam as duas energias: o verde da gosma e o roxo da floresta sagrada. O símbolo em seus escudos não é decoração — é um amplificador de poder.</p>
            <div class="bestiary-tags">
              <span class="tag">Alta resistência</span>
              <span class="tag">Dano elevado</span>
              <span class="tag">Energia dupla</span>
            </div>
          </div>

          <div class="bestiary-card" data-animate="fade-up" data-delay="200">
            <div class="bestiary-header wolf-header">
              <span class="material-symbols-outlined bestiary-icon">pets</span>
              <div class="bestiary-rank">
                <span class="rank-dot"></span><span class="rank-dot"></span><span class="rank-dot empty"></span><span class="rank-dot empty"></span><span class="rank-dot empty"></span>
              </div>
            </div>
            <h3 class="bestiary-name poppins-semibold">Lobos Modificados</h3>
            <p class="bestiary-lore">Guardiões naturais da floresta sagrada, corrompidos pela gosma verde. Seus olhos, antes de um roxo nobre, agora brilham em verde. Disparam esferas de energia — rápidos, mas frágeis se confrontados diretamente.</p>
            <div class="bestiary-tags">
              <span class="tag">Corrompido</span>
              <span class="tag">Ataque à distância</span>
              <span class="tag">Alta velocidade</span>
            </div>
          </div>

          <div class="bestiary-card" data-animate="fade-up" data-delay="300">
            <div class="bestiary-header protetor-header">
              <span class="material-symbols-outlined bestiary-icon">forest</span>
              <div class="bestiary-rank">
                <span class="rank-dot"></span><span class="rank-dot"></span><span class="rank-dot"></span><span class="rank-dot"></span><span class="rank-dot empty"></span>
              </div>
            </div>
            <h3 class="bestiary-name poppins-semibold">O Protetor</h3>
            <p class="bestiary-lore">Criaturas raríssimas da floresta sagrada. Gentis por natureza, seus olhos deveriam ser roxos. Os que servem ao rei têm olhos verdes e uma garra que não deveria existir. Manipulam raízes com força absurda — sinais de uma corrupção profunda e irreversível.</p>
            <div class="bestiary-tags">
              <span class="tag">Chefe médio</span>
              <span class="tag">Vida altíssima</span>
              <span class="tag">Raízes de combate</span>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Capítulo 5: Os Chefes -->
    <div class="historia-chapter chapter-chefes" data-chapter="5">
      <div class="chapter-bg-overlay darker"></div>
      <div class="container">
        <div class="chapter-eyebrow center" data-animate="fade-up">
          <span class="chapter-number">05</span>
          <span class="chapter-label">Os Antagonistas</span>
        </div>
        <h2 class="chapter-title poppins center" data-animate="fade-up">
          Os Guardiões do <span class="gradient-text">Trono Corrompido</span>
        </h2>

        <div class="bosses-layout">
          <div class="boss-card boss-knight" data-animate="fade-up" data-delay="0">
            <div class="boss-bg-glow black-glow"></div>
            <div class="boss-badge">CHEFE</div>
            <div class="boss-icon-wrap">
              <span class="material-symbols-outlined boss-icon">swords</span>
            </div>
            <h3 class="boss-name poppins">O Cavaleiro Negro</h3>
            <p class="boss-title">Guardião Eterno do Rei</p>
            <div class="boss-lore">
              <p>O paciente zero. Antes, o cavaleiro mais leal do reino — tão dedicado que colocou o próprio corpo na frente de uma flecha destinada ao rei. Os curandeiros decretaram sua morte. O rei ofereceu vida.</p>
              <p>O líquido verde o transformou. Sua armadura evoluiu, seu corpo ganhou velocidade e força sobre-humanas. Em gratidão, jurou lealdade eterna. Mas o que o rei deu, o rei pode usar — e o Cavaleiro Negro tornou-se seu instrumento mais preciso.</p>
            </div>
            <div class="boss-abilities">
              <div class="ability-chip"><span class="material-symbols-outlined">bolt</span> Convoca mortos vivos</div>
              <div class="ability-chip"><span class="material-symbols-outlined">add_chart</span> Poder exponencial</div>
              <div class="ability-chip"><span class="material-symbols-outlined">gavel</span> Machado / Espada</div>
            </div>
            <div class="boss-warning">⚠ Não prolongue a batalha — quanto mais tempo durar, mais poderoso ele fica.</div>
          </div>

          <div class="boss-card boss-archer" data-animate="fade-up" data-delay="200">
            <div class="boss-bg-glow archer-glow"></div>
            <div class="boss-badge">CHEFE</div>
            <div class="boss-icon-wrap">
              <span class="material-symbols-outlined boss-icon">target</span>
            </div>
            <h3 class="boss-name poppins">O Arqueiro</h3>
            <p class="boss-title">Cientista das Trevas</p>
            <div class="boss-lore">
              <p>Mais do que um atirador de elite, o Arqueiro foi o cérebro por trás da gosma verde. Liderou a pesquisa, desenvolveu as poções e ajudou o rei e o Cavaleiro Negro a roubarem as raízes roxas da floresta sagrada.</p>
              <p>Diferente dos outros que usam as energias internamente, o Arqueiro as combina diretamente em suas flechas. O resultado: projéteis capazes de explodir montanhas. Antes de partir para a batalha final, entregou uma poção misteriosa ao rei.</p>
            </div>
            <div class="boss-abilities">
              <div class="ability-chip"><span class="material-symbols-outlined">bolt</span> Flechas dupla-energia</div>
              <div class="ability-chip"><span class="material-symbols-outlined">speed</span> Velocidade extrema</div>
              <div class="ability-chip"><span class="material-symbols-outlined">science</span> Flechas especiais</div>
            </div>
            <div class="boss-warning">⚠ Rápido e impreciso, mas uma flecha certeira pode mudar tudo.</div>
          </div>

          <div class="boss-card boss-king" data-animate="fade-up" data-delay="400">
            <div class="boss-bg-glow king-glow"></div>
            <div class="boss-badge king-badge">REI FINAL</div>
            <div class="boss-icon-wrap">
              <span class="material-symbols-outlined boss-icon">crown</span>
            </div>
            <h3 class="boss-name poppins">O Rei</h3>
            <p class="boss-title">O Criador da Corrupção</p>
            <div class="boss-lore">
              <p>O arquiteto de tudo. Criou a gosma verde que ressuscita mortos e concede poder, roubou a energia roxa sagrada da floresta e a misturou com a verde em uma poção exclusiva para si.</p>
              <p>Sob sua armadura escondem-se braços que não são mais humanos — raízes retorcidas de árvore, capazes de se transformar em qualquer coisa que sua vontade ordenar. Ninguém que viu esses braços e o desafiou voltou com vida.</p>
            </div>
            <div class="boss-abilities">
              <div class="ability-chip"><span class="material-symbols-outlined">nature</span> Braços-raízes</div>
              <div class="ability-chip"><span class="material-symbols-outlined">auto_awesome</span> Especiais múltiplos</div>
              <div class="ability-chip"><span class="material-symbols-outlined">visibility_off</span> Poder oculto</div>
            </div>
            <div class="boss-warning">⚠ A poção que recebeu antes da batalha final ainda é um mistério.</div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════
       SEÇÃO MISSÃO
  ═══════════════════════════════════════════════════ -->
  <section class="section-missao" id="missao">
    <div class="missao-bg-layer"></div>
    <div class="container">
      <div class="missao-hero" data-animate="fade-up">
        <span class="section-label">O Objetivo</span>
        <h2 class="section-title poppins">Sua <span class="gradient-text">Missão</span></h2>
      </div>

      <div class="missao-statement" data-animate="fade-up">
        <div class="missao-text-block">
          <p class="missao-lead poppins-semibold">Você é o camponês. Sem título, sem exército, sem magia. Só você, suas habilidades e a determinação de quem tem algo real a salvar.</p>
          <p>O reino foi invadido. A princesa foi capturada. Os campos que você conhecia estão agora infestados de mortos reanimados, lobos corrompidos e cavaleiros que empunham energias que não deveriam existir.</p>
          <p>Cada inimigo que você derrota é um passo em direção ao castelo. Cada chefe que você enfrenta revela mais sobre a corrupção que o rei espalhou. A jornada não é apenas de resgate — é de compreensão. Por que a floresta sagrada foi violada? O que a gosma verde realmente faz? E o que estava naquela poção que o Arqueiro entregou ao rei?</p>
        </div>
      </div>

      <div class="missao-pillars" data-animate="fade-up">
        <div class="pillar">
          <div class="pillar-number poppins">01</div>
          <div class="pillar-content">
            <h3 class="poppins-semibold">Atravessar os Campos Corrompidos</h3>
            <p>Enfrente hordas de esqueletos e lobos modificados que guardam os caminhos até o castelo inimigo. Aprenda os padrões, economize recursos, sobreviva.</p>
          </div>
        </div>
        <div class="pillar-divider"></div>
        <div class="pillar">
          <div class="pillar-number poppins">02</div>
          <div class="pillar-content">
            <h3 class="poppins-semibold">Derrotar os Guardiões do Rei</h3>
            <p>O Arqueiro e o Cavaleiro Negro são obstáculos que o rei colocou entre você e a princesa. São poderosos, são leais, e foram forjados por uma lealdade que só a morte pode quebrar.</p>
          </div>
        </div>
        <div class="pillar-divider"></div>
        <div class="pillar">
          <div class="pillar-number poppins">03</div>
          <div class="pillar-content">
            <h3 class="poppins-semibold">Enfrentar o Rei no Trono</h3>
            <p>A batalha final. O homem que criou a corrupção, que roubou a floresta sagrada e que acredita que pode possuir pessoas como se fossem tesouros. Ele estará com sua poção misteriosa. Esteja pronto para o inesperado.</p>
          </div>
        </div>
        <div class="pillar-divider"></div>
        <div class="pillar">
          <div class="pillar-number poppins">04</div>
          <div class="pillar-content">
            <h3 class="poppins-semibold">Salvar a Princesa</h3>
            <p>Não é apenas um resgate. É uma declaração. É provar que o amor de um camponês tem mais valor do que todo o poder de um rei corrompido. É o fim que eles merecem: um ao lado do outro, livres.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════
       SEÇÃO O TIME
  ═══════════════════════════════════════════════════ -->
  <section class="section-time" id="time">
    <div class="container">
      <div class="section-header" data-animate="fade-up">
        <span class="section-label">Os criadores</span>
        <h2 class="section-title poppins">O <span class="gradient-text">Time</span></h2>
        <p class="section-subtitle">Quatro estudantes que decidiram parar de só jogar e começar a criar. Este projeto é o nosso cartão de visitas.</p>
      </div>

      <div class="time-grid">
        <div class="membro-card" data-animate="fade-up" data-delay="0" v-for="(membro, i) in membros" :key="i">
          <div class="membro-foto-wrap">
            <div class="membro-foto-placeholder" :style="{ background: membro.gradiente }">
              <span class="material-symbols-outlined foto-icon">person</span>
              <span class="foto-hint">Adicionar foto</span>
            </div>
            <div class="membro-glow" :style="{ background: membro.gradiente }"></div>
          </div>
          <div class="membro-info">
            <h3 class="membro-nome poppins-semibold">{{ membro.nome }}</h3>
            <span class="membro-area">{{ membro.area }}</span>
            <div class="membro-matricula">
              <span class="material-symbols-outlined matricula-icon">badge</span>
              <span class="matricula-texto">Matrícula: {{ membro.matricula }}</span>
            </div>
            <p class="membro-desc">{{ membro.descricao }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ═══════════════════════════════════════════════════
       SEÇÃO CONTATO
  ═══════════════════════════════════════════════════ -->
  <section class="section-contato" id="contato">
    <div class="contato-bg-glow"></div>
    <div class="container">
      <div class="section-header" data-animate="fade-up">
        <span class="section-label">Fale conosco</span>
        <h2 class="section-title poppins">Entre em <span class="gradient-text">Contato</span></h2>
        <p class="section-subtitle">Dúvidas sobre o jogo, parcerias ou só quer falar sobre gamedev? A gente ouve.</p>
      </div>

      <div class="contato-layout">
        <div class="contato-info" data-animate="fade-right">
          <div class="contato-item">
            <div class="contato-icon-wrap">
              <span class="material-symbols-outlined">mail</span>
            </div>
            <div>
              <h4 class="poppins-semibold">E-mail do Projeto</h4>
              <p>projeto.camponês@universidade.edu.br</p>
            </div>
          </div>
          <div class="contato-item">
            <div class="contato-icon-wrap">
              <span class="material-symbols-outlined">school</span>
            </div>
            <div>
              <h4 class="poppins-semibold">Instituição</h4>
              <p>Projeto Acadêmico — Desenvolvimento de Jogos</p>
            </div>
          </div>
          <div class="contato-item">
            <div class="contato-icon-wrap">
              <span class="material-symbols-outlined">code</span>
            </div>
            <div>
              <h4 class="poppins-semibold">Repositório</h4>
              <p>github.com/time/campones-jogo</p>
            </div>
          </div>
          <div class="contato-redes">
            <a href="#" class="rede-link">
              <span class="material-symbols-outlined">language</span>
            </a>
            <a href="#" class="rede-link">
              <span class="material-symbols-outlined">smart_display</span>
            </a>
            <a href="#" class="rede-link">
              <span class="material-symbols-outlined">forum</span>
            </a>
          </div>
        </div>

        <form class="contato-form" data-animate="fade-left" @submit.prevent>
          <div class="form-row">
            <div class="form-group">
              <label class="form-label poppins-semibold">Nome</label>
              <input type="text" class="form-input" placeholder="Seu nome" />
            </div>
            <div class="form-group">
              <label class="form-label poppins-semibold">E-mail</label>
              <input type="email" class="form-input" placeholder="seu@email.com" />
            </div>
          </div>
          <div class="form-group">
            <label class="form-label poppins-semibold">Assunto</label>
            <input type="text" class="form-input" placeholder="Sobre o quê você quer falar?" />
          </div>
          <div class="form-group">
            <label class="form-label poppins-semibold">Mensagem</label>
            <textarea class="form-textarea" rows="5" placeholder="Sua mensagem..."></textarea>
          </div>
          <button type="submit" class="btn-primary poppins-semibold form-submit">
            <span class="material-symbols-outlined">send</span>
            Enviar Mensagem
          </button>
        </form>
      </div>
    </div>
  </section>
  
</div>
</template>

<script>
import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";

gsap.registerPlugin(ScrollTrigger);

export default {
  name: 'HomePage',
  data() {
    return {
      membros: [
        {
          nome: 'Nome do Integrante 1',
          area: 'Game Design & Narrativa',
          matricula: '000000',
          descricao: 'Responsável pelo lore, design dos personagens e mecânicas de gameplay.',
          gradiente: 'linear-gradient(135deg, #39ff14, #125f04)'
        },
        {
          nome: 'Nome do Integrante 2',
          area: 'Programação',
          matricula: '000000',
          descricao: 'Desenvolveu os sistemas de combate, IA dos inimigos e arquitetura do jogo.',
          gradiente: 'linear-gradient(135deg, #33cccc, #0a5f5f)'
        },
        {
          nome: 'Nome do Integrante 3',
          area: 'Arte & Animação',
          matricula: '000000',
          descricao: 'Criou os sprites, animações e identidade visual do projeto.',
          gradiente: 'linear-gradient(135deg, #9d39ff, #3a0080)'
        },
        {
          nome: 'Nome do Integrante 4',
          area: 'UI/UX & Som',
          matricula: '000000',
          descricao: 'Projetou a interface do usuário, HUD do jogo e trilha sonora.',
          gradiente: 'linear-gradient(135deg, #ff6b14, #7a2200)'
        }
      ]
    }
  },
  methods: {
    scrollTo(id) {
      const el = document.getElementById(id);
      if (el) el.scrollIntoView({ behavior: 'smooth' });
    },

    animateHero() {
      // Garante que os botões começam visíveis antes do GSAP
      const btn1 = this.$refs.btn1;
      const btn2 = this.$refs.btn2;

      // Define estado inicial via gsap.set (não via tl.to que causava sumiço imediato)
      gsap.set([btn1, btn2], { opacity: 0, scale: 0 });
      gsap.set('.hero-title', { opacity: 0, y: 50 });
      gsap.set('.hero-description', { opacity: 0, y: 30 });
      gsap.set('.scroll-indicator', { opacity: 0 });

      const tl = gsap.timeline({ delay: 0.2 });

      tl.to('.hero-title', {
        y: 0,
        opacity: 1,
        duration: 1,
        ease: 'power3.out'
      })
      .to('.hero-description', {
        y: 0,
        opacity: 1,
        duration: 0.8,
        ease: 'power3.out'
      }, '-=0.5')
      .to([btn1, btn2], {
        scale: 1,
        opacity: 1,
        duration: 0.8,
        stagger: 0.2,
        ease: 'back.out(1.7)',
        clearProps: 'all'
      }, '-=0.4')
      .to('.scroll-indicator', {
        opacity: 1,
        duration: 0.8
      }, '-=0.3');

      // Floating animation for scroll indicator (separate, after reveal)
      tl.add(() => {
        gsap.to('.scroll-indicator', {
          y: 10,
          duration: 1,
          repeat: -1,
          yoyo: true,
          ease: 'sine.inOut'
        });
      });

      this.heroTl = tl;
    },

    initScrollAnimations() {
      // Refresh ScrollTrigger after page layout is done
      ScrollTrigger.refresh();

      // ── data-animate elements ─────────────────────────────
      document.querySelectorAll('[data-animate]').forEach(el => {
        const dir = el.getAttribute('data-animate');
        const delay = parseFloat(el.getAttribute('data-delay') || 0) / 1000;

        const from = { opacity: 0, duration: 0.9, ease: 'power3.out', delay };
        if (dir === 'fade-up')    { from.y = 50; }
        if (dir === 'fade-down')  { from.y = -50; }
        if (dir === 'fade-left')  { from.x = -60; }
        if (dir === 'fade-right') { from.x = 60; }

        gsap.from(el, {
          ...from,
          scrollTrigger: {
            trigger: el,
            start: 'top 88%',
            toggleActions: 'play none none none',
            once: true
          }
        });
      });

      // ── Chapter background parallax ───────────────────────
      document.querySelectorAll('.historia-chapter').forEach(ch => {
        const overlay = ch.querySelector('.chapter-bg-overlay');
        if (!overlay) return;
        gsap.to(overlay, {
          yPercent: 15,
          ease: 'none',
          scrollTrigger: {
            trigger: ch,
            start: 'top bottom',
            end: 'bottom top',
            scrub: true
          }
        });
      });

      // ── Bestiary cards ────────────────────────────────────
      const bestiaryGrid = document.querySelector('.bestiary-grid');
      if (bestiaryGrid) {
        gsap.from('.bestiary-card', {
          y: 60,
          opacity: 0,
          duration: 0.7,
          stagger: 0.12,
          ease: 'power3.out',
          scrollTrigger: {
            trigger: '.bestiary-grid',
            start: 'top 82%',
            once: true
          }
        });
      }

      // ── Boss cards ────────────────────────────────────────
      const bossesLayout = document.querySelector('.bosses-layout');
      if (bossesLayout) {
        gsap.from('.boss-card', {
          y: 80,
          opacity: 0,
          duration: 0.9,
          stagger: 0.18,
          ease: 'power3.out',
          scrollTrigger: {
            trigger: '.bosses-layout',
            start: 'top 82%',
            once: true
          }
        });
      }

      // ── Motivação cards ───────────────────────────────────
      const motivacaoGrid = document.querySelector('.motivacao-grid');
      if (motivacaoGrid) {
        gsap.from('.motivacao-card', {
          y: 50,
          opacity: 0,
          duration: 0.7,
          stagger: 0.1,
          ease: 'power3.out',
          scrollTrigger: {
            trigger: '.motivacao-grid',
            start: 'top 82%',
            once: true
          }
        });
      }

      // ── Mission pillars ───────────────────────────────────
      const missaoPillars = document.querySelector('.missao-pillars');
      if (missaoPillars) {
        gsap.from('.pillar', {
          x: -40,
          opacity: 0,
          duration: 0.8,
          stagger: 0.15,
          ease: 'power3.out',
          scrollTrigger: {
            trigger: '.missao-pillars',
            start: 'top 82%',
            once: true
          }
        });
      }

      // ── Invasion stats ────────────────────────────────────
      const invasionStats = document.querySelector('.invasion-stats');
      if (invasionStats) {
        gsap.from('.stat-item', {
          scale: 0.8,
          opacity: 0,
          duration: 0.6,
          stagger: 0.15,
          ease: 'back.out(1.7)',
          scrollTrigger: {
            trigger: '.invasion-stats',
            start: 'top 85%',
            once: true
          }
        });
      }

      // ── Team cards ────────────────────────────────────────
      const timeGrid = document.querySelector('.time-grid');
      if (timeGrid) {
        gsap.from('.membro-card', {
          y: 60,
          opacity: 0,
          duration: 0.8,
          stagger: 0.15,
          ease: 'power3.out',
          scrollTrigger: {
            trigger: '.time-grid',
            start: 'top 82%',
            once: true
          }
        });
      }

      // ── Section background color shift on scroll ──────────
      const sections = [
        { el: '.section-motivacao', color: '#030f03' },
        { el: '.section-historia',  color: '#000000' },
        { el: '.section-missao',    color: '#030f03' },
        { el: '.section-time',      color: '#000000' },
        { el: '.section-contato',   color: '#030810' }
      ];

      sections.forEach(({ el, color }) => {
        const section = document.querySelector(el);
        if (!section) return;
        ScrollTrigger.create({
          trigger: section,
          start: 'top 50%',
          end: 'bottom 50%',
          onEnter:     () => gsap.to('body', { backgroundColor: color, duration: 1.2, ease: 'power2.inOut' }),
          onEnterBack: () => gsap.to('body', { backgroundColor: color, duration: 1.2, ease: 'power2.inOut' })
        });
      });
    }
  },

  mounted() {
    // Use nextTick + small timeout to guarantee DOM is fully rendered and
    // ScrollTrigger can correctly measure element positions
    this.$nextTick(() => {
      setTimeout(() => {
        this.animateHero();
        //this.initScrollAnimations();
      }, 150);
    });
  },

  unmounted() {
    if (this.heroTl) this.heroTl.kill();
    ScrollTrigger.getAll().forEach(t => t.kill());
    gsap.killTweensOf('*');
  }
}
</script>

<style>
/* ── GLOBAL: CSS custom properties (must not be scoped) ─── */
:root {
  --green-neon: #39ff14;
  --green-dark: #125f04;
  --green-mid: #1a8c05;
  --cyan: #33cccc;
  --purple: #7b2fff;
  --bg-deep: #030f03;
  --bg-black: #000;
  --text-primary: #e8f5e8;
  --text-muted: #8da88d;
  --border-subtle: rgba(57, 255, 20, 0.12);
  --card-bg: rgba(10, 25, 10, 0.85);
}

/* Prevent flash of invisible content before GSAP runs */
.hero-title,
.hero-description,
.scroll-indicator {
  /* GSAP will set these via gsap.set() before animating */
}

@keyframes shine {
  to { background-position: 300% center; }
}
</style>

<style scoped>
/* ─── ROOT WRAPPER ───────────────────────────────────────── */
.home-page-root {
  width: 100%;
  overflow-x: hidden;
}

h1, h2, h3, p {
    font-family: 'Poppins';
}

/* Buttons — GSAP uses gsap.set() for initial invisible state */
.cta-group button {
  will-change: transform, opacity;
}

.hero-section {
  position: relative;
  width: 100%;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  color: #fff;
}
/* Video Background */
.video-container {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -1;
}

.bg-video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* Overlay solicitado: #000 100% na vertical */
.overlay-gradient {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    to bottom,
    rgba(0, 0, 0, 0.2) 0%,
    rgba(0, 0, 0, 0.6) 50%,
    #000000 100%
  );
}

/* Content Layout */
.hero-content {
  text-align: center;
  z-index: 1;
  max-width: 900px;
  padding: 0 20px;
}

.hero-title {
  font-size: clamp(2.5rem, 8vw, 5rem);
  line-height: 1.1;
  margin-bottom: 20px;
  font-weight: 500;
}

/* Letras gradientes com animação de movimento */
.gradient-text {
  background: linear-gradient(
    120deg,
    #33cccc,
    #39ff14,
    #00ff88,
    #33cccc
  );
  background-size: 300% auto;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: shine 5s linear infinite;
}

.hero-description {
  font-size: 1.1rem;
  color: #cbd5e1;
  max-width: 600px;
  margin: 0 auto 40px;
  line-height: 1.6;
}

/* Buttons */
.cta-group {
  display: flex;
  gap: 20px;
  justify-content: center;
}

.btn-primary {
  background: linear-gradient(45deg, #39ff14, #125f04);
  background-size: 200% auto;
  border: none;
  padding: 16px 36px;
  color: white;
  border-radius: 50px;
  cursor: pointer;
  transition: 0.4s;
  box-shadow: 0 10px 20px rgba(3, 148, 92, 0.3);
}

.btn-primary:hover {
  background-position: right center;
  transform: translateY(-3px);
  box-shadow: 0 15px 25px rgba(2, 187, 49, 0.4);
}

.btn-outline {
  background: transparent;
  border: 2px solid rgba(255, 255, 255, 0.3);
  padding: 16px 36px;
  color: white;
  border-radius: 50px;
  cursor: pointer;
  transition: 0.3s;
  backdrop-filter: blur(5px);
}

.btn-outline:hover {
  background: rgba(255, 255, 255, 0.1);
  border-color: white;
}

/* Seta de Scroll */
.scroll-indicator {
  position: absolute;
  bottom: 40px;
  left: 50%;
  transform: translateX(-50%);
  cursor: pointer;
  color: rgba(255, 255, 255, 0.6);
  transition: color 0.3s;
}

.scroll-indicator span {
  font-size: 3rem;
}

.scroll-indicator:hover {
  color: #33cccc;
}

/* Font helpers */
.poppins-regular { font-family: 'Poppins', sans-serif; font-weight: 400; }
.poppins-semibold { font-family: 'Poppins', sans-serif; font-weight: 600; }
.poppins-bold { font-family: 'Poppins', sans-serif; font-weight: 700; }

/* ─── CONTAINERS & LAYOUT ────────────────────────────────── */
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 40px;
}

.section-label {
  display: inline-block;
  font-family: 'Poppins', sans-serif;
  font-size: 0.7rem;
  font-weight: 600;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: var(--green-neon);
  border: 1px solid rgba(57, 255, 20, 0.3);
  padding: 4px 14px;
  border-radius: 20px;
  margin-bottom: 20px;
}

.section-title {
  font-size: clamp(2rem, 4vw, 3rem);
  line-height: 1.1;
  color: var(--text-primary);
  margin-bottom: 16px;
  font-weight: 500;
}

.section-subtitle {
  font-family: 'Poppins', sans-serif;
  font-size: 1rem;
  color: var(--text-muted);
  max-width: 600px;
  line-height: 1.7;
}

.section-header {
  text-align: center;
  margin-bottom: 64px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.gradient-text {
  background: linear-gradient(120deg, #33cccc, #39ff14, #00ff88, #33cccc);
  background-size: 300% auto;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: shine 5s linear infinite;
}

.gradient-text-red {
  background: linear-gradient(120deg, #ff4444, #ff8800, #ff4444);
  background-size: 300% auto;
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: shine 5s linear infinite;
}

/* ─── MOTIVAÇÃO ──────────────────────────────────────────── */
.section-motivacao {
  position: relative;
  padding: 120px 0;
  background: var(--bg-deep);
  overflow: hidden;
}

.section-bg-particles {
  position: absolute;
  inset: 0;
  background-image:
    radial-gradient(circle at 20% 20%, rgba(57, 255, 20, 0.04) 0%, transparent 50%),
    radial-gradient(circle at 80% 80%, rgba(51, 204, 204, 0.04) 0%, transparent 50%);
  pointer-events: none;
}

.motivacao-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 24px;
}

.motivacao-card {
  background: var(--card-bg);
  border: 1px solid var(--border-subtle);
  border-radius: 16px;
  padding: 32px 28px;
  position: relative;
  overflow: hidden;
  transition: transform 0.3s ease, border-color 0.3s ease, box-shadow 0.3s ease;
  backdrop-filter: blur(10px);
}

.motivacao-card::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 1px;
  background: linear-gradient(90deg, transparent, rgba(57, 255, 20, 0.4), transparent);
}

.motivacao-card:hover {
  transform: translateY(-6px);
  border-color: rgba(57, 255, 20, 0.3);
  box-shadow: 0 20px 60px rgba(57, 255, 20, 0.08);
}

.card-featured {
  background: linear-gradient(135deg, rgba(18, 95, 4, 0.3), rgba(10, 25, 10, 0.9));
  border-color: rgba(57, 255, 20, 0.3);
  grid-row: span 1;
}

.card-icon-wrapper {
  position: relative;
  width: 52px;
  height: 52px;
  margin-bottom: 20px;
}

.card-icon {
  font-size: 2rem;
  color: var(--green-neon);
  position: relative;
  z-index: 1;
}

.icon-glow {
  position: absolute;
  inset: -10px;
  background: radial-gradient(circle, rgba(57, 255, 20, 0.15) 0%, transparent 70%);
  border-radius: 50%;
}

.icon-glow.green {
  background: radial-gradient(circle, rgba(57, 255, 20, 0.25) 0%, transparent 70%);
}

.card-title {
  font-size: 1.05rem;
  color: var(--text-primary);
  margin-bottom: 12px;
}

.card-text {
  font-family: 'Poppins', sans-serif;
  font-size: 0.875rem;
  color: var(--text-muted);
  line-height: 1.7;
  margin-bottom: 20px;
}

.card-tag {
  display: inline-block;
  font-family: 'Poppins', sans-serif;
  font-size: 0.65rem;
  font-weight: 600;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--text-muted);
  border: 1px solid var(--border-subtle);
  padding: 3px 10px;
  border-radius: 20px;
}

.card-tag.featured {
  color: var(--green-neon);
  border-color: rgba(57, 255, 20, 0.4);
}

/* ─── HISTÓRIA ───────────────────────────────────────────── */
.section-historia {
  position: relative;
  background: var(--bg-black);
}

.historia-chapter {
  position: relative;
  padding: 120px 0;
  overflow: hidden;
}

.chapter-bg-overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(135deg, rgba(3, 15, 3, 0.95) 0%, rgba(0,0,0,0.85) 100%);
  z-index: 0;
}

.chapter-bg-overlay.dark {
  background: linear-gradient(135deg, rgba(0,0,0,0.98) 0%, rgba(5, 20, 5, 0.9) 100%);
}

.chapter-bg-overlay.red {
  background: linear-gradient(135deg, rgba(20, 3, 3, 0.97) 0%, rgba(0,0,0,0.9) 100%);
}

.chapter-bg-overlay.deep {
  background: linear-gradient(135deg, rgba(2, 8, 20, 0.98) 0%, rgba(5, 2, 20, 0.9) 100%);
}

.chapter-bg-overlay.darker {
  background: linear-gradient(135deg, rgba(0,0,0,0.99) 0%, rgba(5, 5, 5, 0.99) 100%);
}

.chapter-content {
  position: relative;
  z-index: 1;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 80px;
  align-items: center;
}

.chapter-content.reverse {
  direction: rtl;
}

.chapter-content.reverse > * {
  direction: ltr;
}

.chapter-eyebrow {
  display: flex;
  align-items: center;
  gap: 14px;
  margin-bottom: 20px;
}

.chapter-eyebrow.center {
  justify-content: center;
}

.chapter-number {
  font-family: 'Poppins', sans-serif;
  font-size: 0.75rem;
  font-weight: 700;
  color: var(--green-neon);
  letter-spacing: 0.1em;
}

.chapter-label {
  font-family: 'Poppins', sans-serif;
  font-size: 0.7rem;
  font-weight: 600;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: var(--text-muted);
}

.chapter-title {
  font-size: clamp(1.8rem, 3.5vw, 2.8rem);
  line-height: 1.15;
  color: var(--text-primary);
  margin-bottom: 28px;
  font-weight: 500;
}

.chapter-title.center {
  text-align: center;
}

.chapter-subtitle {
  font-family: 'Poppins', sans-serif;
  font-size: 0.95rem;
  color: var(--text-muted);
  max-width: 700px;
  margin: 0 auto 64px;
  text-align: center;
  line-height: 1.7;
}

.chapter-body p {
  font-family: 'Poppins', sans-serif;
  font-size: 0.9rem;
  color: var(--text-muted);
  line-height: 1.8;
  margin-bottom: 16px;
}

.chapter-quote {
  margin-top: 32px;
  padding: 24px 32px;
  border-left: 3px solid var(--green-neon);
  background: rgba(57, 255, 20, 0.04);
  border-radius: 0 12px 12px 0;
}

.chapter-quote blockquote {
  font-family: 'Poppins', sans-serif;
  font-size: 0.95rem;
  font-style: italic;
  color: var(--text-primary);
  line-height: 1.7;
  margin: 0;
}

.chapter-visual {
  display: flex;
  justify-content: center;
  align-items: center;
}

.visual-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 16px;
  padding: 48px;
  background: var(--card-bg);
  border: 1px solid var(--border-subtle);
  border-radius: 20px;
  backdrop-filter: blur(10px);
}

.visual-icon {
  font-size: 4rem;
  color: var(--green-neon);
  opacity: 0.7;
}

.visual-label {
  font-family: 'Poppins', sans-serif;
  font-size: 0.8rem;
  color: var(--text-muted);
  letter-spacing: 0.1em;
}

.lore-cards-stack {
  display: flex;
  flex-direction: column;
  gap: 16px;
  width: 100%;
  max-width: 320px;
}

.lore-mini-card {
  display: flex;
  align-items: center;
  gap: 14px;
  padding: 18px 24px;
  background: var(--card-bg);
  border: 1px solid var(--border-subtle);
  border-radius: 12px;
  font-family: 'Poppins', sans-serif;
  font-size: 0.85rem;
  color: var(--text-muted);
  transition: all 0.3s;
}

.lore-mini-card .material-symbols-outlined {
  color: var(--text-muted);
  font-size: 1.2rem;
}

.lore-mini-card.active {
  border-color: rgba(57, 255, 20, 0.4);
  color: var(--text-primary);
  background: linear-gradient(135deg, rgba(18, 95, 4, 0.3), var(--card-bg));
}

.lore-mini-card.active .material-symbols-outlined {
  color: var(--green-neon);
}

/* Invasion stats */
.invasion-stats {
  display: flex;
  gap: 40px;
  margin-top: 48px;
  flex-wrap: wrap;
}

.stat-item {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 4px;
}

.stat-icon {
  color: var(--green-neon);
  font-size: 1.4rem;
  margin-bottom: 4px;
}

.stat-value {
  font-family: 'Poppins', sans-serif;
  font-size: 1.8rem;
  font-weight: 700;
  color: var(--text-primary);
  line-height: 1;
}

.stat-label {
  font-family: 'Poppins', sans-serif;
  font-size: 0.75rem;
  color: var(--text-muted);
  max-width: 160px;
  line-height: 1.4;
}

/* Bestiary */
.bestiary-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
  position: relative;
  z-index: 1;
}

.bestiary-card {
  background: var(--card-bg);
  border: 1px solid var(--border-subtle);
  border-radius: 16px;
  padding: 28px 22px;
  transition: transform 0.3s, border-color 0.3s, box-shadow 0.3s;
  backdrop-filter: blur(10px);
}

.bestiary-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 24px 60px rgba(57, 255, 20, 0.1);
  border-color: rgba(57, 255, 20, 0.25);
}

.bestiary-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 16px;
  padding-bottom: 16px;
  border-bottom: 1px solid var(--border-subtle);
}

.bestiary-icon {
  font-size: 1.6rem;
  color: var(--green-neon);
}

.skeleton-header .bestiary-icon { color: #aaa; }
.knight-header .bestiary-icon { color: var(--cyan); }
.wolf-header .bestiary-icon { color: var(--green-neon); }
.protetor-header .bestiary-icon { color: var(--purple); }

.bestiary-rank {
  display: flex;
  gap: 4px;
}

.rank-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: var(--green-neon);
}

.rank-dot.empty {
  background: transparent;
  border: 1px solid rgba(57, 255, 20, 0.25);
}

.bestiary-name {
  font-size: 0.95rem;
  color: var(--text-primary);
  margin-bottom: 12px;
}

.bestiary-lore {
  font-family: 'Poppins', sans-serif;
  font-size: 0.78rem;
  color: var(--text-muted);
  line-height: 1.7;
  margin-bottom: 16px;
}

.bestiary-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
}

.tag {
  font-family: 'Poppins', sans-serif;
  font-size: 0.6rem;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--text-muted);
  border: 1px solid var(--border-subtle);
  padding: 2px 8px;
  border-radius: 20px;
}

/* Boss cards */
.bosses-layout {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 28px;
  position: relative;
  z-index: 1;
}

.boss-card {
  background: var(--card-bg);
  border: 1px solid var(--border-subtle);
  border-radius: 20px;
  padding: 36px 28px;
  position: relative;
  overflow: hidden;
  transition: transform 0.3s, border-color 0.3s;
  backdrop-filter: blur(12px);
}

.boss-card:hover {
  transform: translateY(-8px);
  border-color: rgba(57, 255, 20, 0.3);
}

.boss-bg-glow {
  position: absolute;
  top: -40px;
  right: -40px;
  width: 200px;
  height: 200px;
  border-radius: 50%;
  filter: blur(60px);
  opacity: 0.3;
  pointer-events: none;
}

.black-glow { background: radial-gradient(#444, transparent); }
.archer-glow { background: radial-gradient(var(--cyan), transparent); }
.king-glow { background: radial-gradient(var(--purple), transparent); }

.boss-badge {
  display: inline-block;
  font-family: 'Poppins', sans-serif;
  font-size: 0.6rem;
  font-weight: 700;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  padding: 4px 12px;
  border-radius: 20px;
  background: rgba(57, 255, 20, 0.1);
  border: 1px solid rgba(57, 255, 20, 0.3);
  color: var(--green-neon);
  margin-bottom: 20px;
}

.king-badge {
  background: rgba(123, 47, 255, 0.15);
  border-color: rgba(123, 47, 255, 0.4);
  color: #b87fff;
}

.boss-icon-wrap {
  width: 60px;
  height: 60px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 16px;
  background: rgba(57, 255, 20, 0.06);
  border: 1px solid var(--border-subtle);
  margin-bottom: 18px;
}

.boss-icon {
  font-size: 2rem;
  color: var(--green-neon);
}

.boss-king .boss-icon { color: #b87fff; }
.boss-archer .boss-icon { color: var(--cyan); }

.boss-name {
  font-size: 1.2rem;
  color: var(--text-primary);
  margin-bottom: 4px;
  font-weight: 500;
}

.boss-title {
  font-family: 'Poppins', sans-serif;
  font-size: 0.75rem;
  color: var(--green-neon);
  letter-spacing: 0.08em;
  margin-bottom: 20px;
  display: block;
}

.boss-lore p {
  font-family: 'Poppins', sans-serif;
  font-size: 0.82rem;
  color: var(--text-muted);
  line-height: 1.7;
  margin-bottom: 10px;
}

.boss-abilities {
  display: flex;
  flex-direction: column;
  gap: 8px;
  margin: 20px 0;
}

.ability-chip {
  display: flex;
  align-items: center;
  gap: 8px;
  font-family: 'Poppins', sans-serif;
  font-size: 0.78rem;
  color: var(--text-muted);
  padding: 8px 12px;
  background: rgba(57, 255, 20, 0.04);
  border: 1px solid var(--border-subtle);
  border-radius: 8px;
}

.ability-chip .material-symbols-outlined {
  font-size: 1rem;
  color: var(--green-neon);
}

.boss-warning {
  font-family: 'Poppins', sans-serif;
  font-size: 0.75rem;
  color: #ff8800;
  padding: 10px 14px;
  background: rgba(255, 136, 0, 0.06);
  border: 1px solid rgba(255, 136, 0, 0.2);
  border-radius: 8px;
  line-height: 1.5;
}

/* ─── MISSÃO ─────────────────────────────────────────────── */
.section-missao {
  position: relative;
  padding: 120px 0;
  background: var(--bg-deep);
  overflow: hidden;
}

.missao-bg-layer {
  position: absolute;
  inset: 0;
  background:
    radial-gradient(ellipse at 10% 50%, rgba(57, 255, 20, 0.03) 0%, transparent 60%),
    radial-gradient(ellipse at 90% 50%, rgba(51, 204, 204, 0.03) 0%, transparent 60%);
  pointer-events: none;
}

.missao-hero {
  text-align: center;
  margin-bottom: 64px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.missao-statement {
  max-width: 800px;
  margin: 0 auto 72px;
  padding: 40px;
  background: var(--card-bg);
  border: 1px solid var(--border-subtle);
  border-radius: 20px;
  backdrop-filter: blur(10px);
  position: relative;
  z-index: 1;
}

.missao-statement::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 2px;
  background: linear-gradient(90deg, transparent, var(--green-neon), transparent);
  border-radius: 2px 2px 0 0;
}

.missao-lead {
  font-family: 'Poppins', sans-serif;
  font-size: 1.1rem;
  color: var(--text-primary);
  line-height: 1.6;
  margin-bottom: 16px;
}

.missao-text-block p {
  font-family: 'Poppins', sans-serif;
  font-size: 0.9rem;
  color: var(--text-muted);
  line-height: 1.8;
  margin-bottom: 14px;
}

.missao-pillars {
  position: relative;
  z-index: 1;
  display: flex;
  flex-direction: column;
  gap: 0;
}

.pillar {
  display: grid;
  grid-template-columns: 80px 1fr;
  gap: 32px;
  align-items: flex-start;
  padding: 40px 0;
}

.pillar-divider {
  height: 1px;
  background: var(--border-subtle);
  margin: 0;
}

.pillar-number {
  font-size: 2.5rem;
  font-weight: 700;
  color: rgba(57, 255, 20, 0.15);
  line-height: 1;
  padding-top: 4px;
}

.pillar-content h3 {
  font-size: 1rem;
  color: var(--text-primary);
  margin-bottom: 10px;
}

.pillar-content p {
  font-family: 'Poppins', sans-serif;
  font-size: 0.875rem;
  color: var(--text-muted);
  line-height: 1.7;
}

/* ─── O TIME ─────────────────────────────────────────────── */
.section-time {
  padding: 120px 0;
  background: var(--bg-black);
  overflow: hidden;
}

.time-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 24px;
}

.membro-card {
  background: var(--card-bg);
  border: 1px solid var(--border-subtle);
  border-radius: 20px;
  padding: 32px 24px;
  text-align: center;
  transition: transform 0.3s, border-color 0.3s, box-shadow 0.3s;
  backdrop-filter: blur(10px);
  position: relative;
  overflow: hidden;
}

.membro-card::before {
  content: '';
  position: absolute;
  bottom: 0; left: 0; right: 0;
  height: 1px;
  background: linear-gradient(90deg, transparent, rgba(57, 255, 20, 0.3), transparent);
}

.membro-card:hover {
  transform: translateY(-8px);
  border-color: rgba(57, 255, 20, 0.3);
  box-shadow: 0 24px 60px rgba(57, 255, 20, 0.08);
}

.membro-foto-wrap {
  position: relative;
  width: 100px;
  height: 100px;
  margin: 0 auto 24px;
}

.membro-foto-placeholder {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 2px;
  cursor: pointer;
  transition: transform 0.3s;
  position: relative;
  z-index: 1;
}

.membro-foto-placeholder:hover {
  transform: scale(1.05);
}

.foto-icon {
  font-size: 2rem;
  color: rgba(255,255,255,0.9);
}

.foto-hint {
  font-family: 'Poppins', sans-serif;
  font-size: 0.55rem;
  color: rgba(255,255,255,0.7);
  letter-spacing: 0.05em;
}

.membro-glow {
  position: absolute;
  inset: -10px;
  border-radius: 50%;
  filter: blur(20px);
  opacity: 0.25;
  z-index: 0;
}

.membro-nome {
  font-size: 1rem;
  color: var(--text-primary);
  margin-bottom: 6px;
}

.membro-area {
  display: inline-block;
  font-family: 'Poppins', sans-serif;
  font-size: 0.65rem;
  font-weight: 600;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--green-neon);
  margin-bottom: 14px;
}

.membro-matricula {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 6px;
  margin-bottom: 14px;
  padding: 6px 12px;
  background: rgba(57, 255, 20, 0.04);
  border: 1px solid var(--border-subtle);
  border-radius: 8px;
}

.matricula-icon {
  font-size: 0.9rem;
  color: var(--text-muted);
}

.matricula-texto {
  font-family: 'Poppins', sans-serif;
  font-size: 0.72rem;
  color: var(--text-muted);
  letter-spacing: 0.05em;
}

.membro-desc {
  font-family: 'Poppins', sans-serif;
  font-size: 0.78rem;
  color: var(--text-muted);
  line-height: 1.6;
}

/* ─── CONTATO ────────────────────────────────────────────── */
.section-contato {
  position: relative;
  padding: 120px 0;
  background: var(--bg-deep);
  overflow: hidden;
}

.contato-bg-glow {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 600px;
  height: 600px;
  background: radial-gradient(circle, rgba(57, 255, 20, 0.03) 0%, transparent 70%);
  pointer-events: none;
}

.contato-layout {
  display: grid;
  grid-template-columns: 1fr 1.5fr;
  gap: 80px;
  align-items: flex-start;
}

.contato-info {
  display: flex;
  flex-direction: column;
  gap: 28px;
}

.contato-item {
  display: flex;
  gap: 18px;
  align-items: flex-start;
}

.contato-icon-wrap {
  width: 44px;
  height: 44px;
  border-radius: 12px;
  background: rgba(57, 255, 20, 0.06);
  border: 1px solid var(--border-subtle);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
}

.contato-icon-wrap .material-symbols-outlined {
  font-size: 1.2rem;
  color: var(--green-neon);
}

.contato-item h4 {
  font-size: 0.85rem;
  color: var(--text-primary);
  margin-bottom: 4px;
}

.contato-item p {
  font-family: 'Poppins', sans-serif;
  font-size: 0.8rem;
  color: var(--text-muted);
}

.contato-redes {
  display: flex;
  gap: 12px;
  margin-top: 8px;
}

.rede-link {
  width: 44px;
  height: 44px;
  border-radius: 12px;
  background: var(--card-bg);
  border: 1px solid var(--border-subtle);
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--text-muted);
  transition: all 0.3s;
  text-decoration: none;
}

.rede-link:hover {
  border-color: rgba(57, 255, 20, 0.4);
  color: var(--green-neon);
  background: rgba(57, 255, 20, 0.06);
}

.rede-link .material-symbols-outlined {
  font-size: 1.1rem;
}

/* Form */
.contato-form {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.form-row {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
}

.form-group {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.form-label {
  font-size: 0.78rem;
  color: var(--text-primary);
  letter-spacing: 0.05em;
}

.form-input,
.form-textarea {
  background: var(--card-bg);
  border: 1px solid var(--border-subtle);
  border-radius: 10px;
  padding: 12px 16px;
  color: var(--text-primary);
  font-family: 'Poppins', sans-serif;
  font-size: 0.875rem;
  transition: border-color 0.3s, box-shadow 0.3s;
  outline: none;
  resize: vertical;
}

.form-input::placeholder,
.form-textarea::placeholder {
  color: var(--text-muted);
}

.form-input:focus,
.form-textarea:focus {
  border-color: rgba(57, 255, 20, 0.4);
  box-shadow: 0 0 0 3px rgba(57, 255, 20, 0.06);
}

.form-submit {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  background: linear-gradient(45deg, #39ff14, #125f04);
  background-size: 200% auto;
  border: none;
  padding: 16px 36px;
  color: white;
  border-radius: 50px;
  cursor: pointer;
  transition: 0.4s;
  box-shadow: 0 10px 20px rgba(3, 148, 92, 0.3);
  font-size: 0.875rem;
}

.form-submit:hover {
  background-position: right center;
  transform: translateY(-3px);
  box-shadow: 0 15px 25px rgba(2, 187, 49, 0.4);
}

.form-submit .material-symbols-outlined {
  font-size: 1.1rem;
}

/* ─── FOOTER ─────────────────────────────────────────────── */
.site-footer {
  padding: 48px 0;
  background: var(--bg-black);
  border-top: 1px solid var(--border-subtle);
}

.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.footer-brand {
  display: flex;
  flex-direction: column;
  gap: 4px;
}

.footer-title {
  font-size: 1rem;
  color: var(--text-primary);
  font-weight: 600;
}

.footer-sub {
  font-family: 'Poppins', sans-serif;
  font-size: 0.72rem;
  color: var(--text-muted);
}

.footer-copy {
  font-family: 'Poppins', sans-serif;
  font-size: 0.75rem;
  color: var(--text-muted);
}
</style>