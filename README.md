<p align="center">
  <img src="media/nexus-cockpit.jpg" alt="CR404 NEXUS — das Cockpit" width="100%">
</p>

<h1 align="center">CR404 NEXUS</h1>

<p align="center">
  <strong>Eine Super-App. Fünf Geschäfte. Ein Schaltpult.</strong><br>
  Öffentliches Dossier für Kunden und Investoren. Kein Quellcode.
</p>

<p align="center">
  <a href="#warum-das-haelt">Warum das hält</a> ·
  <a href="#die-fuenf">Die fünf</a> ·
  <a href="#einzeln">Einzeln kaufbar</a> ·
  <a href="#kapital">Wohin Kapital geht</a> ·
  <a href="docs/INVESTORS.en.md">English</a>
</p>

---

Die Bilder in diesem Repository sind **Markenstills**, keine Screenshots.
Sie zeigen die Haltung des Produkts, nicht eine vorgetäuschte Oberfläche.
Die Implementierung liegt in privaten Arbeitsrepos und wird hier absichtlich nicht mitgeliefert.

Wer NEXUS in einer Minute verstehen will, liest nur diesen Absatz:

> CR404 NEXUS ist das Betriebssystem für kleine, automatisierbare Geschäfte.
> Handel, Laden, Wächter, App-Fabrik und Studio hängen an einem Cockpit.
> Jedes Modul ist ein eigenes Produkt. Zusammen rechnen sie auf eine Kasse.

<p align="center">
  <img src="media/constellation.jpg" alt="Sechs Teile, eine Mitte" width="100%">
</p>

---

## Warum das hält

Die meisten „Super-Apps“ sind ein Dashboard mit zu vielen Tabs.
NEXUS ist anders geschnitten: **die Grenzen sind schon Repos.**

| | |
| --- | --- |
| **Suite oder Einzelstück** | Ein Händler nimmt Tante Emma und lässt den Krypto-Desk liegen. Ein Builder nimmt nur Forge. Die Suite ist das Upsell, nicht die Eintrittskarte. |
| **Eine Kasse** | Was die Module verdienen, ist im Cockpit als eine Treasury gedacht. Heute als ehrliches Modell. Morgen als echte Buchung, sobald ein Mandant und eine Lizenzfrage geklärt sind. |
| **Der Mensch bleibt im Loop** | Listings, Deploys und Echtgeld-Orders sind Entwürfe, bis jemand freigibt. Das ist kein fehlendes Feature. Das ist der Grund, warum ein vorsichtiger Kunde das überhaupt anfasst. |
| **Keys sind optional** | Das Cockpit läuft ohne API-Schlüssel. Schlüssel schalten Live-Kurse, Börsen-Guthaben und die KI frei. Sie sind nicht die Krücke, an der alles hängt. |
| **Kein stiller Bot mit Kundengeld** | Dagobert ist ein Entscheidungs- und Simulationscockpit. Echtgeld sitzt hinter einem Gate. Schlüssel gehören auf den Server, nie in den Browser. |

Der Reiz für einen Investor ist nicht „noch ein Agent“.
Der Reiz ist ein **Baukasten mit eigenen Märkten**, der sich Modul für Modul finanzieren lässt, ohne die Suite zu zerlegen.

---

## Die fünf

Kurz. Danach jeder Teil so, dass man ihn auch ohne die anderen versteht.
Ausführlicher, falls du es jemandem schickst, der nur ein Modul will: die Seiten unter [`docs/`](docs/).

| Modul | In einem Satz | Allein lebensfähig | Heute |
| --- | --- | --- | --- |
| [RoboCop404](#robocop404) | Der Wächter. Start, Stopp, Audit, Circuit Breaker. | Ja, als Ops- und Security-Modul | Cockpit plus schlankes Security-Modul |
| [Tante Emma](#tante-emma) | Der Laden. B2C-Shop und B2B-Dropshipping mit Freigabe. | Ja | Fläche und Modell stehen, Marktplätze sind Skelette |
| [Dagobert Market](#dagobert-market) | Der Desk. Signale, Paper-Trade, Backtest. Krypto zuerst. | Ja | Dashboard läuft, Echtgeld ist verriegelt |
| [Forge](#forge) | Die Fabrik. Aus einem Satz wird eine lauffähige App. | Ja | Pipeline baut, testet und committet lokal |
| [Music Video Studio](#music-video-studio) | Das Studio. Track, Bild, Clip — aus einem Prompt. | Ja, sobald der Generator steht | Platz im Cockpit, Generator ist der nächste Bau |

Dazu, leiser, aber schon geschnitten: **AL Messenger** (Chat für Shop, Support und Agenten), die **B2B-Arbitrage-Engine** (Discovery, SEO, Freigabe vor dem Listing) und **CR404 Shops** (die Verkaufsseiten, aus denen Tante Emma das Sortiment zieht). Sie sind Zulieferer der fünf, keine sechste Story. Wer sie einzeln will, kann sie einzeln haben. Siehe [Einzeln](#einzeln).

---

## RoboCop404

<p align="center">
  <img src="media/robocop.jpg" alt="RoboCop404 — der Wächter" width="100%">
</p>

RoboCop404 ist nicht der Film und nicht ein Mensch in Rüstung.
Es ist der Operator, der aufpasst, während der Rest arbeitet.

**Was er tut**

- Nimmt Strategien entgegen, die woanders entworfen wurden — zum Beispiel aus dem Taktik-Regal von Dagobert — und lässt sie in einer Schleife weiterlaufen.
- Kann gestartet und gestoppt werden. Wenn das Risiko kippt, zieht er den **Circuit Breaker**. Lieber still als teuer.
- Darunter liegt ein kleines, regelbasiertes Security-Modul ohne Sprachmodell und ohne externe Abhängigkeit: System- und Secret-Audit (nur lesen), Stacktrace-Analyse mit Empfehlung, Deployment nur als **Entwurf**. Ausrollen braucht eine Freigabe.

**Warum das ein Produkt ist**

Teams, die Agenten laufen lassen, kaufen nicht „mehr Intelligenz“.
Sie kaufen jemanden, der den Stecker zieht.
Allein verkauft ist RoboCop404 ein Ops-Modul: Audit, Debug-Hinweis, Deploy-Entwurf, Not-Aus.
In der Suite ist er das Schloss an Dagobert, Forge und dem Shop.

Ausführlich: [`docs/robocop.md`](docs/robocop.md)

---

## Tante Emma

<p align="center">
  <img src="media/tante-emma.jpg" alt="Tante Emma — Laden und B2B" width="100%">
</p>

Tante Emma ist der Laden an der Ecke, der nebenbei Großhandel kann.
Zwei Geschäfte, eine Theke.

**B2C — der Shop**

Sortiment, Warenkorb, Kasse, Bestellhistorie.
Der klassische Verkauf, den ein lokaler Händler ohne Agentur anfassen kann.

**B2B und Dropshipping — der Desk dahinter**

- Artikel finden: Trend, günstig, oder nach Vorgabe.
- Einkauf gegen Verkauf legen, Marge sehen, Status führen.
- SEO-Text dazu: Titel, Beschreibung, Keywords. Regelbasiert, bei Bedarf mit KI geschärft.
- Vorschau des Listings, bevor es irgendwo öffentlich wird.
- Bestellung, Tracking, Kasse.
- Marktplatz-Anschluss als Richtung: Amazon, eBay, Shopify, Etsy, Kaufland. **Immer über offizielle APIs. Immer mit menschlicher Freigabe vor dem Listing.**

Der Gewinn, den der Shop als verkauft oder versandt markiert, ist im NEXUS-Cockpit der gemeinsamen Treasury zugeordnet.
Ohne NEXUS ist Tante Emma trotzdem ein eigener Shop mit eigenem B2B-Desk und angeschlossenem Messenger für Support.

**Ehrlich zum Stand**

Die Fläche und das Produktmodell stehen: Finder, Artikel, Vergleich, Bestellungen, Tracking, Kasse, lokaler Shop, Setup.
Katalog, Warenkorb und SEO sind als Backend angelegt.
Die Marktplatz-Publisher sind Skelette, kein stiller Autopilot, der nachts auf Amazon listet.
Genau das will ein vernünftiger Händler auch nicht, bevor er die Freigabe gesehen hat.

Ausführlich: [`docs/tante-emma.md`](docs/tante-emma.md)

---

## Dagobert Market

<p align="center">
  <img src="media/dagobert-market.jpg" alt="Dagobert Market — der Desk" width="100%">
</p>

Dagobert Market ist der Schreibtisch für Märkte.
Zuerst Krypto. Daneben der Blick auf Aktien, Rohstoffe, Forex und Edelmetalle.

**Was auf dem Tisch liegt**

- Signale: kaufen, halten, verkaufen. Mit Begründung, nicht mit einem Ampel-Kult.
- Marktübersicht und Charts, technische Indikatoren.
- Portfolio und Paper-Trade. Simulation, bevor irgendjemand echtes Geld anfasst.
- Eine Bibliothek von Taktiken: SMA, EMA, RSI, MACD, Bollinger, Momentum, Grid und Kombinationen. Jede lässt sich backtesten — Rendite, Anzahl Trades, gegen Buy-and-Hold, Equity-Kurve — und an RoboCop übergeben.
- KI-Analyse nur über ein Backend. Der Schlüssel liegt nie im Browser.
- Wallet-Anbindung lesend: CoinGecko ohne Schlüssel, FRED für Makro, Kraken und Binance nur für Guthaben, nur serverseitig.

**Was es nicht ist**

Keine Börse. Kein Broker. Keine Lizenzbehauptung. Keine Rendite.
Echtgeld-Orders laufen nur, wenn ein eigener serverseitiger Endpunkt hinterlegt ist **und** der Handel ausdrücklich bestätigt wurde.
Ohne Netzwerk fällt der Desk auf Beispieldaten zurück und bleibt bedienbar.
Allein ist Dagobert ein Entscheidungs- und Simulationscockpit für Leute, die eine Meinung zum Markt wollen, bevor sie eine Order wollen.
In der Suite ist er der Marktarm, dessen Papiergewinne die Treasury als Modell kennt — nicht als versprochenes Vermögen.

Ausführlich: [`docs/dagobert-market.md`](docs/dagobert-market.md)

---

## Forge

<p align="center">
  <img src="media/forge.jpg" alt="Forge — die App-Fabrik" width="100%">
</p>

Forge baut Software auf Zuruf.
Nicht als Folie. Als Projekt.

Fünf Rollen, eine Pipeline:

| Rolle | Aufgabe |
| --- | --- |
| **Architect** | Aus dem Satz wird Struktur und Stack. |
| **Builder** | Frontend und Backend. Echte Routen, nicht eine Attrappe. |
| **Styler** | Layout, das man anfassen kann. |
| **Tester** | Startet, was gebaut wurde, und prüft, ob es antwortet. |
| **Shipper** | Legt ein lokales Git-Commit. Push nur, wenn es jemand ausdrücklich sagt. |

Forge kennt die Geschwister als Vorlagen: AL Messenger, Tante Emma, Music Video Studio, eine schlichte Landingpage.
Es kann sie anfassen, anpassen und als neues Projekt ausgeben.

**Ehrlich zum Stand**

Ein Auftrag wie „bau eine Landingpage für …“ erzeugt lauffähigen Code, startet das generierte Backend und committet lokal.
Der Styler hat noch ein festes Theme, nicht eines pro Auftrag.
Der Push in ein echtes Remote ist bewusst aus. Nichts veröffentlicht sich selbst.

Allein ist Forge eine App-Fabrik für Leute, die aus einem Satz eine Fläche wollen, die wirklich hochfährt.
In der Suite ist Forge die Werkbank, die neue Module in dieselbe Familie legt, ohne die Namen der anderen zu zertrampeln.

Ausführlich: [`docs/forge.md`](docs/forge.md)

---

## Music Video Studio

<p align="center">
  <img src="media/musicvideo-studio.jpg" alt="Music Video Studio" width="100%">
</p>

Das Studio ist der kreative Arm.
Ein Prompt wird Track, Loop oder Stem. Dazu Bild: Visualizer, Lyric-Video, Clip.

Im Cockpit hat es schon einen Platz. Streams und ein RPM-Umsatz sind als Modell an die gemeinsame Kasse gehängt, damit man sehen kann, wie ein Kreativgeschäft in derselben Bilanz sitzt wie Shop und Desk.
Das ist eine Produktentscheidung, kein belegter Katalog und keine Stream-Zahl.

**Was es werden soll, allein**

Ein Studio für Creator und kleine Labels: Musik und Bild aus einem Auftrag, Warteschlange für die schweren Jobs, Ablage lokal oder S3-kompatibel.
Forge kann das Studio als Vorlage ausliefern. NEXUS muss dafür nicht an sein.

**Ehrlich zum Stand**

Architektur und der Platz im Cockpit stehen.
Die Generator-Anbindung ist der nächste Bauabschnitt, nicht ein fertiger Knopf.
Wer heute investiert, investiert in die Strecke vom Prompt zur Datei — nicht in einen vorgetäuschten Hit.

Ausführlich: [`docs/musicvideo-studio.md`](docs/musicvideo-studio.md)

---

## Einzeln

Man muss die Suite nicht wollen.

| Wenn du nur das brauchst | Nimmst du | Und lässt liegen |
| --- | --- | --- |
| Einen Laden plus Dropshipping mit Freigabe | Tante Emma | Desk, Studio, Forge |
| Einen Markt-Desk mit Paper-Trade | Dagobert Market | Shop, Studio |
| Jemanden, der Agenten beaufsichtigt | RoboCop404 | alles andere |
| Software aus einem Satz | Forge | Handel und Shop |
| Tracks und Clips | Music Video Studio | den Rest |
| Nur Chat, Support, Channels | AL Messenger | die Geschäfte |
| Nur Produktsuche, SEO, Listing-Freigabe | B2B-Arbitrage | den Laden drumherum |
| Nur die Verkaufsseiten | CR404 Shops | den B2B-Desk |

Jedes Modul hat einen eigenen Namensraum. Sie beißen sich nicht, wenn man sie später doch zusammensteckt.
Der Kleber in der Suite ist langweilig und genau deshalb richtig: ein gemeinsamer Zustand, ein Event-Bus, eine Treasury, ein Schalter pro Modul.

Wie die Übergabe gedacht ist, ohne Code zu zeigen: [`docs/standalone.md`](docs/standalone.md)

---

## Was ein Kunde kauft

Keine Zeilen. Eine Arbeit, die er heute von Hand oder von fünf Tools macht.

- **Der Händler** sucht Artikel, rechnet Marge, schreibt Texte, scheut sich, blind zu listen. Tante Emma legt ihm die Vorschau hin und wartet.
- **Der Trader** will eine Meinung, einen Backtest und einen Not-Aus, bevor er eine Börse anfasst. Dagobert plus RoboCop.
- **Die Agentur oder der Gründer** will aus einem Satz eine Fläche, die hochfährt. Forge.
- **Der Creator** will Ton und Bild aus einem Auftrag, nicht aus zwölf Abos. Das Studio, sobald die Generatoren stehen.
- **Der Betreiber** will alles auf einem Schirm und eine Zahl, die sagt, was die Teile zusammen tragen. Das ist NEXUS.

---

## Kapital

Dieses Repository ist kein Term Sheet und keine Runde.
Es ist die Landkarte, worauf Geld arbeiten würde.

1. **Tante Emma zu Ende bringen.** Von der stehenden Fläche zu echten, freigabepflichtigen Marktplatz-Verbindungen. Ein Händler, ein Marktplatz, ein Listing, das ein Mensch gesehen hat. Dann der zweite.
2. **Dagobert sauber halten.** Bessere Daten, nachvollziehbare Backtests, das Echtgeld-Gate juristisch und technisch langweilig machen. Nicht „wir traden Kundengeld“.
3. **Forge wiederholbar machen.** Ein Theme pro Auftrag. Eine Auslieferung, die ein Kunde ohne den Autor starten kann.
4. **Studio: Prompt zu Datei.** Eine Generator-Strecke, eine Warteschlange, eine Ablage. Ein Clip, den man abspielt.
5. **NEXUS: ein Mandant.** Login, echte Kasse, getrennte Kunden. Heute ist das Cockpit lokal, offline-fähig und ehrlich simulierbar. Der Sprung ist nicht mehr Architektur. Der Sprung ist Betrieb.

Wer nur ein Modul finanzieren will, kann das. Die Repos sind schon getrennt.
Wer die Hülle finanziert, finanziert den Kleber und die Kasse, nicht noch einmal jedes Geschäft.

---

## Was heute schon steht

Nicht als Versprechen. Als Inventur.

- Ein Browser-Cockpit für NEXUS: Launcher, Treasury, Wallet, Ideen-Cockpit, Autopilot als Simulation, alle Module anklickbar.
- Neun fachliche Agenten im Kern: Nischen, Startups, Bitcoin-Signal, Rohstoffe, Portfolio, Datenbündelung, Code-Qualität, Security-Scan, Affiliate- und B2B-Entwürfe. Reports als JSON und Markdown. Ein Agent, der scheitert, reißt den Lauf nicht mit.
- RoboCop404 als Fläche plus regelbasiertes Security-Modul mit Freigabe vor dem Deploy.
- Tante Emma als Shop- und B2B-Fläche, Backend angelegt, Messenger angedockt.
- Dagobert Market als Trading-Dashboard mit Paper-Trade, Taktik-Backtest und verriegeltem Echtgeld.
- Forge als Pipeline, die wirklich baut, startet und lokal committet.
- AL Messenger als eigenständiger Chat mit Räumen, Presence und WebSocket-Hub.
- Music Video Studio als Architektur und Cockpit-Platz.

Was nicht steht, steht oben bei jedem Modul. Es wird hier nicht weichgezeichnet.

---

## Was bewusst nicht in diesem Repo liegt

Kein Anwendungscode. Keine Abhängigkeiten. Keine Schlüssel. Keine `.env`.
Keine Kopie der Arbeitsrepos.

Dieses Verzeichnis ist die öffentliche Fläche: Texte, Stills, die Karte.
Zugang zur Implementierung gibt es im Gespräch, nicht über einen öffentlichen Klon.
Die privaten Arbeitsrepos bleiben die Werkstatt. Dieses Repo bleibt das Schaufenster.

---

## Gespräch

GitHub: [@arondakoa](https://github.com/arondakoa)

Englisch, kürzer, für jemanden der nicht auf Deutsch liest: [`docs/INVESTORS.en.md`](docs/INVESTORS.en.md)

---

<sub>

Kein Angebot von Wertpapieren. Keine Anlageberatung. Keine Einladung, Geld zu überweisen.
Handel und Krypto können auf null gehen. Ob ein Modul eine Erlaubnis braucht, hängt vom Land ab und davon, ob fremdes Geld bewegt wird. Stand dieses Dossiers ist Dagobert ein Simulations- und Entscheidungskockpit mit gesperrtem Echtgeld-Pfad.
Markenstills sind Stimmung, nicht die ausgelieferte Oberfläche.
RoboCop404 ist ein eigener Produktname und kein Bezug auf einen Film.

</sub>
