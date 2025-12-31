<!DOCTYPE html>
<html lang="sk">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>bez-bullshitu.org</title>

  <style>
    :root {
      --bg: #0b0e13;
      --panel: rgba(18, 21, 28, 0.85);
      --border: #242a38;
      --text: #e6e9ef;
      --muted: #9aa3b2;
      --accent: #b9c4ff;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      min-height: 100vh;
      font-family: Inter, system-ui, -apple-system, Segoe UI, Roboto, sans-serif;
      color: var(--text);
      background:
        radial-gradient(900px 500px at 15% 20%, rgba(120,140,255,.12), transparent 55%),
        radial-gradient(900px 600px at 85% 30%, rgba(180,120,255,.10), transparent 55%),
        linear-gradient(180deg, #0a0c11 0%, var(--bg) 100%);
    }

    .container {
      max-width: 1100px;
      margin: 0 auto;
      padding: 64px 24px 80px;
    }

    /* HERO */
    .hero {
      margin-bottom: 48px;
    }

    .brand {
      font-size: 12px;
      letter-spacing: .28em;
      text-transform: uppercase;
      color: var(--muted);
      margin-bottom: 14px;
    }

    h1 {
      font-size: 56px;
      line-height: 1.05;
      letter-spacing: -0.4px;
      margin-bottom: 16px;
    }

    .lead {
      font-size: 18px;
      color: var(--muted);
      max-width: 70ch;
      margin-bottom: 22px;
    }

    .chips {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
    }

    .chip {
      border: 1px solid var(--border);
      background: rgba(18,21,28,.6);
      padding: 8px 12px;
      border-radius: 999px;
      font-size: 13px;
      color: var(--accent);
    }

    /* GRID */
    .grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 22px;
      margin-top: 28px;
    }

    .card {
      background: var(--panel);
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 26px;
      box-shadow: 0 12px 40px rgba(0,0,0,.45);
      backdrop-filter: blur(10px);
    }

    .lang {
      font-size: 12px;
      letter-spacing: .22em;
      text-transform: uppercase;
      color: var(--muted);
      margin-bottom: 14px;
    }

    .card p {
      margin-bottom: 14px;
      line-height: 1.65;
    }

    .sub {
      margin-top: 18px;
      font-weight: 600;
      color: var(--accent);
    }

    ul {
      list-style: none;
      margin: 10px 0 14px;
    }

    li {
      padding-left: 16px;
      margin-bottom: 6px;
      position: relative;
    }

    li::before {
      content: "–";
      position: absolute;
      left: 0;
      color: var(--muted);
    }

    .muted {
      color: var(--muted);
      font-size: 14px;
    }

    /* FOOTER */
    .footer {
      margin-top: 40px;
      padding-top: 18px;
      border-top: 1px solid var(--border);
      display: flex;
      gap: 16px;
      flex-wrap: wrap;
      font-size: 14px;
      color: var(--muted);
    }

    @media (max-width: 900px) {
      h1 { font-size: 40px; }
      .grid { grid-template-columns: 1fr; }
    }
  </style>
</head>

<body>
  <main class="container">

    <section class="hero">
      <div class="brand">bez-bullshitu.org</div>

      <h1>
        Ticho.<br>
        Presne.<br>
        Neodvratne.
      </h1>

      <p class="lead">
        Nie sme názor. Sme metóda. Dôkaz → rozklad → verdikt.
      </p>

      <div class="chips">
        <span class="chip">Citácia</span>
        <span class="chip">Dáta</span>
        <span class="chip">Logika</span>
        <span class="chip">Verdikt</span>
      </div>
    </section>

    <section class="grid">
      <article class="card">
        <div class="lang">SK</div>

        <p>Táto stránka neprezentuje názory. Neobhajuje postoje. Nezastupuje ideológiu.</p>
        <p>Jej účelom je analyzovať tvrdenia a porovnávať ich s dostupnými faktami a kontextom.</p>

        <p class="sub">Každý rozbor je postavený na:</p>
        <ul>
          <li>citovanom tvrdení</li>
          <li>overiteľných dátach</li>
          <li>logickom rozklade</li>
          <li>jasne formulovanom verdikte</li>
        </ul>

        <p><strong>Verdikt nie je názor.</strong> Je výsledkom analýzy.</p>
        <p class="muted">Ak je tvrdenie pravdivé, obstojí. Ak nie, rozpadne sa samo.</p>
      </article>

      <article class="card">
        <div class="lang">EN</div>

        <p>This site does not present opinions. It does not defend positions. It does not represent an ideology.</p>
        <p>Its purpose is to analyze claims and compare them with available facts and context.</p>

        <p class="sub">Each analysis is based on:</p>
        <ul>
          <li>a quoted claim</li>
          <li>verifiable data</li>
          <li>logical decomposition</li>
          <li>a clearly formulated verdict</li>
        </ul>

        <p><strong>A verdict is not an opinion.</strong> It is the result of analysis.</p>
        <p class="muted">If a claim is true, it will stand. If not, it will collapse on its own.</p>
      </article>
    </section>

    <footer class="footer">
      <span>Method over noise.</span>
      <span>Evidence over vibes.</span>
      <span>No ads. No agenda. No mercy for bullshit.</span>
    </footer>
    <p style="margin-top:24px; font-size:14px; opacity:.8;">
  Kontakt: <a href="mailto:kontakt@bez-bullshitu.org">kontakt@bez-bullshitu.org</a>
</p>

  </main>
</body>
</html>

