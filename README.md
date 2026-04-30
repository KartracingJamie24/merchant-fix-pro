<!DOCTYPE html>
<html xmlns:o="urn:schemas-microsoft-com:office:office"
      xmlns:w="urn:schemas-microsoft-com:office:word"
      xmlns="http://www.w3.org/TR/REC-html40"
      lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <!--[if gte mso 9]>
  <xml>
    <w:WordDocument>
      <w:View>Print</w:View>
      <w:Zoom>100</w:Zoom>
      <w:DoNotOptimizeForBrowser/>
    </w:WordDocument>
  </xml>
  <![endif]-->
  <title>Modul 1 – Grundlagen & Setup</title>
  <style>
    /* ===== WORD-OPTIMIERTE STILE ===== */
    @page {
      size: A4;
      margin: 2.5cm 2cm 2.5cm 2cm;
      mso-header-margin: 1cm;
      mso-footer-margin: 1cm;
    }

    body {
      font-family: 'Calibri', Arial, sans-serif;
      font-size: 11pt;
      color: #1a1a1a;
      background: #ffffff;
      line-height: 1.6;
      margin: 0;
      padding: 0;
    }

    /* ===== KOPFZEILE ===== */
    .header {
      border-bottom: 3px solid #1a73e8;
      padding-bottom: 15px;
      margin-bottom: 30px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .header-logo {
      font-size: 22pt;
      font-weight: 900;
      color: #1a73e8;
      letter-spacing: 1px;
    }

    .header-info {
      text-align: right;
      font-size: 9pt;
      color: #666;
    }

    /* ===== TITELSEITE ===== */
    .title-page {
      text-align: center;
      padding: 40px 20px 50px;
      background: linear-gradient(135deg, #f8f9ff, #e8f0fe);
      border-radius: 12px;
      margin-bottom: 40px;
      border: 2px solid #1a73e8;
      page-break-after: always;
    }

    .kurs-badge {
      display: inline-block;
      background: #1a73e8;
      color: white;
      padding: 6px 18px;
      border-radius: 20px;
      font-size: 10pt;
      font-weight: 700;
      margin-bottom: 20px;
      letter-spacing: 1px;
      text-transform: uppercase;
    }

    .title-page h1 {
      font-size: 32pt;
      font-weight: 900;
      color: #1a1a1a;
      margin: 15px 0 10px;
      line-height: 1.2;
    }

    .title-page .modul-nummer {
      font-size: 16pt;
      color: #1a73e8;
      font-weight: 700;
      margin-bottom: 8px;
    }

    .title-page .subtitle {
      font-size: 14pt;
      color: #555;
      margin-bottom: 25px;
    }

    .title-divider {
      width: 80px;
      height: 4px;
      background: #1a73e8;
      margin: 20px auto;
      border-radius: 2px;
    }

    .title-meta {
      font-size: 10pt;
      color: #888;
      margin-top: 20px;
    }

    /* ===== INHALTSVERZEICHNIS ===== */
    .toc {
      background: #f8f9ff;
      border: 1px solid #e0e7ff;
      border-left: 5px solid #1a73e8;
      border-radius: 8px;
      padding: 25px 30px;
      margin-bottom: 40px;
      page-break-after: always;
    }

    .toc h2 {
      font-size: 16pt;
      color: #1a73e8;
      margin-bottom: 15px;
      font-weight: 800;
    }

    .toc ol {
      margin: 0;
      padding-left: 20px;
    }

    .toc ol li {
      font-size: 11pt;
      margin-bottom: 8px;
      color: #333;
    }

    .toc ol li a {
      color: #1a73e8;
      text-decoration: none;
    }

    /* ===== ÜBERSCHRIFTEN ===== */
    h1 {
      font-family: 'Calibri', Arial, sans-serif;
      font-size: 28pt;
      font-weight: 900;
      color: #1a1a1a;
      margin-top: 30px;
      margin-bottom: 10px;
      border-bottom: 2px solid #1a73e8;
      padding-bottom: 8px;
    }

    h2 {
      font-family: 'Calibri', Arial, sans-serif;
      font-size: 18pt;
      font-weight: 800;
      color: #1a73e8;
      margin-top: 25px;
      margin-bottom: 10px;
    }

    h3 {
      font-family: 'Calibri', Arial, sans-serif;
      font-size: 14pt;
      font-weight: 700;
      color: #333;
      margin-top: 18px;
      margin-bottom: 8px;
    }

    /* ===== ABSÄTZE & LISTEN ===== */
    p {
      font-size: 11pt;
      margin-bottom: 12px;
      color: #333;
    }

    ul {
      margin-left: 20px;
      margin-bottom: 15px;
    }

    ul li {
      font-size: 11pt;
      margin-bottom: 6px;
      color: #333;
    }

    ol {
      margin-left: 20px;
      margin-bottom: 15px;
    }

    ol li {
      font-size: 11pt;
      margin-bottom: 8px;
      color: #333;
    }

    /* ===== INFO-BOX ===== */
    .info-box {
      background: #e8f4fd;
      border: 1px solid #bee3f8;
      border-left: 5px solid #1a73e8;
      border-radius: 6px;
      padding: 15px 20px;
      margin: 20px 0;
    }

    .info-box strong {
      color: #1a73e8;
      font-size: 11pt;
    }

    /* ===== TIPP-BOX ===== */
    .tipp-box {
      background: #f0fff4;
      border: 1px solid #c6f6d5;
      border-left: 5px solid #38a169;
      border-radius: 6px;
      padding: 15px 20px;
      margin: 20px 0;
    }

    .tipp-box strong {
      color: #38a169;
      font-size: 11pt;
    }

    /* ===== WARNUNG-BOX ===== */
    .warn-box {
      background: #fffbeb;
      border: 1px solid #fbd38d;
      border-left: 5px solid #d69e2e;
      border-radius: 6px;
      padding: 15px 20px;
      margin: 20px 0;
    }

    .warn-box strong {
      color: #d69e2e;
      font-size: 11pt;
    }

    /* ===== FEHLER-TABELLE ===== */
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 20px 0;
      font-size: 10pt;
    }

    table th {
      background: #1a73e8;
      color: white;
      padding: 10px 14px;
      text-align: left;
      font-weight: 700;
    }

    table td {
      padding: 9px 14px;
      border-bottom: 1px solid #e0e0e0;
      vertical-align: top;
    }

    table tr:nth-child(even) td {
      background: #f8f9ff;
    }

    table tr:hover td {
      background: #e8f0fe;
    }

    /* ===== SCHRITT-KARTEN ===== */
    .schritt-card {
      background: #f8f9ff;
      border: 1px solid #e0e7ff;
      border-radius: 10px;
      padding: 18px 22px;
      margin-bottom: 16px;
      position: relative;
    }

    .schritt-nummer {
      display: inline-block;
      background: #1a73e8;
      color: white;
      width: 30px;
      height: 30px;
      border-radius: 50%;
      text-align: center;
      line-height: 30px;
      font-weight: 800;
      font-size: 13pt;
      margin-right: 10px;
    }

    .schritt-title {
      font-size: 13pt;
      font-weight: 700;
      color: #1a1a1a;
    }

    /* ===== CHECKLISTE ===== */
    .checkliste {
      background: #f0fff4;
      border: 2px solid #38a169;
      border-radius: 10px;
      padding: 25px 30px;
      margin: 30px 0;
      page-break-before: always;
    }

    .checkliste h2 {
      color: #38a169;
      font-size: 18pt;
      margin-bottom: 20px;
    }

    .check-item {
      display: flex;
      align-items: flex-start;
      gap: 12px;
      margin-bottom: 14px;
      padding: 10px 15px;
      background: white;
      border: 1px solid #c6f6d5;
      border-radius: 8px;
    }

    .check-box {
      width: 20px;
      height: 20px;
      border: 2px solid #38a169;
      border-radius: 4px;
      flex-shrink: 0;
      margin-top: 1px;
    }

    .check-text {
      font-size: 11pt;
      color: #333;
    }

    .check-text strong {
      color: #1a1a1a;
    }

    .check-text small {
      display: block;
      color: #888;
      font-size: 9pt;
      margin-top: 2px;
    }

    /* ===== FUSSZEILE ===== */
    .footer {
      border-top: 2px solid #1a73e8;
      padding-top: 12px;
      margin-top: 50px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 9pt;
      color: #888;
    }

    .footer a {
      color: #1a73e8;
    }

    /* ===== SEITENUMBRUCH ===== */
    .page-break {
      page-break-after: always;
    }

    /* ===== DRUCK-OPTIMIERUNG ===== */
    @media print {
      body { margin: 0; }
      .no-print { display: none; }
      h1, h2, h3 { page-break-after: avoid; }
      .schritt-card { page-break-inside: avoid; }
      .check-item { page-break-inside: avoid; }
    }
  </style>
</head>
<body>

<!-- ===== KOPFZEILE ===== -->
<div class="header">
  <div class="header-logo">
    🏎️ KartracinJamie24
  </div>
  <div class="header-info">
    Google Merchant &amp; Shopify Meisterkurs<br>
    Modul 1 | Version 1.0 | April 2026
  </div>
</div>

<!-- ===== TITELSEITE ===== -->
<div class="title-page">
  <div class="kurs-badge">📘 Google Merchant &amp; Shopify Meisterkurs</div>
  <div class="modul-nummer">MODUL 1</div>
  <h1>Grundlagen &amp; Setup</h1>
  <div class="subtitle">Google Merchant Konto erstellen &amp; Shopify verbinden</div>
  <div class="title-divider"></div>
  <p style="color:#555; font-size:12pt; max-width:500px; margin:0 auto 20px;">
    In diesem Modul lernst du Schritt für Schritt, wie du dein Google Merchant Center Konto
    einrichtest und erfolgreich mit deinem Shopify-Shop verbindest – auch als kompletter Anfänger!
  </p>
  <div class="title-meta">
    🏎️ KartracinJamie24 &nbsp;|&nbsp; Version 1.0 &nbsp;|&nbsp; April 2026 &nbsp;|&nbsp;
    support@merchant-fix-pro.de
  </div>
</div>

<!-- ===== INHALTSVERZEICHNIS ===== -->
<div class="toc">
  <h2>📋 Inhaltsverzeichnis</h2>
  <ol>
    <li>Zielsetzung dieses Moduls</li>
    <li>Was du brauchst – Voraussetzungen</li>
    <li>Schritt-für-Schritt-Anleitung</li>
    <li>Häufige Stolpersteine &amp; Sofort-Lösungen</li>
    <li>✅ Checkliste Modul 1 (Druckversion)</li>
  </ol>
</div>

<!-- ===== ABSCHNITT 1: ZIELSETZUNG ===== -->
<h1>1. Zielsetzung</h1>

<p>
  Herzlich willkommen zu Modul 1 des <strong>Google Merchant &amp; Shopify Meisterkurses</strong>!
  In diesem ersten Modul legst du das Fundament für deinen Erfolg mit Google Shopping.
</p>

<div class="info-box">
  <strong>🎯 Ziel dieses Moduls:</strong><br>
  Nach diesem Modul hast du ein vollständig eingerichtetes Google Merchant Center Konto,
  das erfolgreich mit deinem Shopify-Shop verbunden ist und deinen ersten Produktfeed synchronisiert.
</div>

<p>Nach diesem Modul kannst du:</p>
<ul>
  <li>✅ Ein Google Merchant Center Konto von Grund auf einrichten</li>
  <li>✅ Shopify sicher und korrekt mit Google Merchant verbinden</li>
  <li>✅ Deinen ersten Produktfeed erstellen und synchronisieren</li>
  <li>✅ Die wichtigsten Richtlinien kennen und einhalten</li>
  <li>✅ Typische Anfängerfehler von Beginn an vermeiden</li>
</ul>

<div class="tipp-box">
  <strong>💡 Tipp:</strong>
  Arbeite dieses Modul von Anfang bis Ende durch, bevor du weitermachst.
  Eine solide Grundlage spart dir später stundenlange Fehlersuche!
</div>

<div class="page-break"></div>

<!-- ===== ABSCHNITT 2: VORAUSSETZUNGEN ===== -->
<h1>2. Voraussetzungen</h1>

<p>Bevor du startest, stelle sicher, dass du folgendes bereit hast:</p>

<table>
  <tr>
    <th>✅ Was du brauchst</th>
    <th>📝 Details</th>
    <th>⚡ Wichtigkeit</th>
  </tr>
  <tr>
    <td><strong>Google-Konto</strong></td>
    <td>Aktives Gmail- oder Google Workspace Konto</td>
    <td>🔴 Pflicht</td>
  </tr>
  <tr>
    <td><strong>Shopify-Shop</strong></td>
    <td>Aktiver Shop mit Admin-Rechten</td>
    <td>🔴 Pflicht</td>
  </tr>
  <tr>
    <td><strong>Verifizierte Domain</strong></td>
    <td>Domain muss dir gehören und erreichbar sein</td>
    <td>🔴 Pflicht</td>
  </tr>
  <tr>
    <td><strong>Mindest. 1 Produkt</strong></td>
    <td>Zum Testen des Feeds benötigt</td>
    <td>🟡 Empfohlen</td>
  </tr>
  <tr>
    <td><strong>GTIN / EAN-Codes</strong></td>
    <td>Barcodes deiner Produkte (falls vorhanden)</td>
    <td>🟡 Empfohlen</td>
  </tr>
  <tr>
    <td><strong>Rechtliche Texte</strong></td>
    <td>Impressum, Datenschutz, Widerrufsbelehrung</td>
    <td>🔴 Pflicht</td>
  </tr>
  <tr>
    <td><strong>Produktbilder</strong></td>
    <td>Mind. 800×800 px, klarer Hintergrund</td>
    <td>🔴 Pflicht</td>
  </tr>
</table>

<div class="warn-box">
  <strong>⚠️ Achtung:</strong>
  Ohne verifizierte Domain und vollständige rechtliche Texte wird Google dein Konto
  nicht aktivieren oder sogar sperren. Stelle sicher, dass diese Punkte vorab erfüllt sind!
</div>

<div class="page-break"></div>

<!-- ===== ABSCHNITT 3: SCHRITT-FÜR-SCHRITT ===== -->
<h1>3. Schritt-für-Schritt-Anleitung</h1>

<div class="info-box">
  <strong>ℹ️ Hinweis:</strong>
  Führe jeden Schritt der Reihe nach aus. Überspringe keinen Schritt,
  da jeder auf dem vorherigen aufbaut.
</div>

<h2>SCHRITT 1: Google Merchant Center Konto erstellen</h2>

<div class="schritt-card">
  <span class="schritt-nummer">1</span>
  <span class="schritt-title">Merchant Center öffnen</span>
  <p style="margin-top:10px; margin-bottom:0;">
    Öffne deinen Browser und gehe zu:
    <strong>merchants.google.com</strong><br>
    Klicke auf <em>„Jetzt starten"</em> oder <em>„Konto erstellen"</em>.
  </p>
</div>

<div class="schritt-card">
  <span class="schritt-nummer">2</span>
  <span class="schritt-title">Mit Google-Konto anmelden</span>
  <p style="margin-top:10px; margin-bottom:0;">
    Melde dich mit deinem <strong>Google-Konto</strong> an.
    Empfehlung: Nutze dasselbe Konto, das du auch für Google Ads verwenden willst.
  </p>
</div>

<div class="schritt-card">
  <span class="schritt-nummer">3</span>
  <span class="schritt-title">Unternehmensdaten eingeben</span>
  <p style="margin-top:10px; margin-bottom:0;">
    Fülle alle Felder des Assistenten aus:
  </p>
  <ul style="margin-top:8px;">
    <li><strong>Unternehmensname:</strong> Exakt wie im Impressum angegeben</li>
    <li><strong>Land:</strong> Deutschland (oder dein Verkaufsland)</li>
    <li><strong>Währung:</strong> Euro (EUR)</li>
    <li><strong>Zeitzone:</strong> Europe/Berlin</li>
  </ul>
</div>

<div class="schritt-card">
  <span class="schritt-nummer">4</span>
  <span class="schritt-title">Website verifizieren</span>
  <p style="margin-top:10px; margin-bottom:0;">
    Google muss bestätigen, dass du der Inhaber der Website bist.
    Wähle eine dieser Methoden:
  </p>
  <ul style="margin-top:8px;">
    <li><strong>HTML-Tag:</strong> Meta-Tag in den &lt;head&gt; deiner Website einfügen</li>
    <li><strong>HTML-Datei:</strong> Datei ins Root-Verzeichnis hochladen</li>
    <li><strong>DNS:</strong> TXT-Eintrag beim Domain-Anbieter hinzufügen</li>
    <li><strong>Google Tag Manager:</strong> Falls bereits vorhanden</li>
  </ul>
</div>

<div class="tipp-box">
  <strong>💡 Tipp für Shopify-Nutzer:</strong>
  In Shopify gehst du zu <em>Online Shop → Themes → Code bearbeiten → theme.liquid</em>
  und fügst den Meta-Tag direkt nach dem &lt;head&gt;-Tag ein.
</div>

<h2>SCHRITT 2: Google &amp; YouTube App in Shopify installieren</h2>

<div class="schritt-card">
  <span class="schritt-nummer">1</span>
  <span class="schritt-title">Shopify Admin öffnen</span>
  <p style="margin-top:10px; margin-bottom:0;">
    Logge dich in deinen Shopify Admin ein unter <strong>deinshop.myshopify.com/admin</strong>
  </p>
</div>

<div class="schritt-card">
  <span class="schritt-nummer">2</span>
  <span class="schritt-title">App suchen und installieren</span>
  <p style="margin-top:10px; margin-bottom:0;">
    Gehe zu <strong>Apps → App Store</strong> und suche nach:
    <em>„Google &amp; YouTube"</em><br>
    Klicke auf <strong>„Installieren"</strong> und bestätige die Berechtigungen.
  </p>
</div>

<div class="schritt-card">
  <span class="schritt-nummer">3</span>
  <span class="schritt-title">Mit Google-Konto verbinden</span>
  <p style="margin-top:10px; margin-bottom:0;">
    Nach der Installation öffnet sich ein Verbindungsassistent.<br>
    Klicke auf <strong>„Mit Google verbinden"</strong> und wähle dein Google-Konto.
  </p>
</div>

<div class="schritt-card">
  <span class="schritt-nummer">4</span>
  <span class="schritt-title">Merchant Center verknüpfen</span>
  <p style="margin-top:10px; margin-bottom:0;">
    Wähle dein bereits erstelltes <strong>Merchant Center Konto</strong> aus der Liste.<br>
    Falls noch nicht vorhanden, kannst du es direkt hier erstellen.
  </p>
</div>

<h2>SCHRITT 3: Produktfeed synchronisieren</h2>

<div class="schritt-card">
  <span class="schritt-nummer">1</span>
  <span class="schritt-title">Produkte auswählen</span>
  <p style="margin-top:10px; margin-bottom:0;">
    Wähle aus, welche Produkte du bei Google Shopping listen möchtest.
    Du kannst alle Produkte oder bestimmte Collections wählen.
  </p>
</div>

<div class="schritt-card">
  <span class="schritt-nummer">2</span>
  <span class="schritt-title">Ersten Sync starten</span>
  <p style="margin-top:10px; margin-bottom:0;">
    Klicke auf <strong>„Sync starten"</strong>.
    Der erste Sync kann 15–30 Minuten dauern.
    Google prüft anschließend deine Produkte (24–72 Stunden).
  </p>
</div>

<div class="warn-box">
  <strong>⚠️ Wichtig:</strong>
  Ändere keine Produktdaten während des ersten Syncs.
  Warte, bis der Sync vollständig abgeschlossen ist.
</div>

<div class="page-break"></div>

<!-- ===== ABSCHNITT 4: STOLPERSTEINE ===== -->
<h1>4. Häufige Stolpersteine &amp; Sofort-Lösungen</h1>

<p>Diese Fehler begegnen fast jedem Anfänger. Hier sind die direkten Lösungen:</p>

<table>
  <tr>
    <th>#</th>
    <th>❌ Problem</th>
    <th>✅ Sofort-Lösung</th>
  </tr>
  <tr>
    <td><strong>1</strong></td>
    <td>Website nicht verifiziert</td>
    <td>Meta-Tag oder DNS-Eintrag hinzufügen (Schritt 1.4)</td>
  </tr>
  <tr>
    <td><strong>2</strong></td>
    <td>Produkte werden abgelehnt</td>
    <td>Titel und Beschreibung prüfen, GTIN ergänzen</td>
  </tr>
  <tr>
    <td><strong>3</strong></td>
    <td>Fehlende GTIN / MPN</td>
    <td>EAN-Code beim Hersteller anfragen oder selbst generieren</td>
  </tr>
  <tr>
    <td><strong>4</strong></td>
    <td>Preisabweichung im Feed</td>
    <td>Feed-Sync neu starten, Preis im Shop prüfen</td>
  </tr>
  <tr>
    <td><strong>5</strong></td>
    <td>Bildqualität zu niedrig</td>
    <td>Bilder auf mind. 800×800 px hochskalieren</td>
  </tr>
  <tr>
    <td><strong>6</strong></td>
    <td>App verbindet sich nicht</td>
    <td>Browser-Cache leeren, neuen Tab öffnen, neu versuchen</td>
  </tr>
  <tr>
    <td><strong>7</strong></td>
    <td>Konto wird nicht aktiviert</td>
    <td>Alle Pflichtfelder prüfen, rechtliche Texte ergänzen</td>
  </tr>
  <tr>
    <td><strong>8</strong></td>
    <td>Sync läuft nicht durch</td>
    <td>Internetverbindung prüfen, App neu installieren</td>
  </tr>
</table>

<div class="tipp-box">
  <strong>💡 Profi-Tipp:</strong>
  Gehe im Merchant Center zu <em>Diagnose</em> → dort siehst du alle aktuellen
  Fehler mit genauen Beschreibungen. Nutze diese Seite als erste Anlaufstelle bei Problemen!
</div>

<div class="page-break"></div>

<!-- ===== CHECKLISTE ===== -->
<div class="checkliste">
  <h2>✅ Checkliste Modul 1 – Grundlagen &amp; Setup</h2>
  <p style="color:#555; margin-bottom:20px;">
    Hake jeden Punkt ab, bevor du mit Modul 2 weitermachst!
  </p>

  <div class="check-item">
    <div class="check-box"></div>
    <div class="check-text">
      <strong>Google Merchant Center Konto erstellt</strong>
      <small>Account unter merchants.google.com angelegt und Basisdaten ausgefüllt</small>
    </div>
  </div>

  <div class="check-item">
    <div class="check-box"></div>
    <div class="check-text">
      <strong>Website verifiziert und beansprucht</strong>
      <small>Meta-Tag, HTML-Datei oder DNS-Eintrag hinzugefügt</small>
    </div>
  </div>

  <div class="check-item">
    <div class="check-box"></div>
    <div class="check-text">
      <strong>Google &amp; YouTube App in Shopify installiert</strong>
      <small>App aus dem
