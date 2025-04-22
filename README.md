# UmbracoWebShopExample

**Case: Umbraco / Frontend Developer**

Dette projekt er en mini-moderne produktside bygget med **Umbraco CMS (v15.3.1)** og **Tailwind CSS** som en del af en caseopgave.
---

## 🛠️ Brugt teknologi

- **Umbraco CMS v15.3.1**
- **.NET 7**
- **Tailwind CSS v3**
- **Alpine.js v3**
- **Git & GitHub for version control**

---

### 1. Umbraco Setup

#### Document Types Created:

- `Produkt`
  - `Produktnavn` (Text)
  - `Beskrivelse` (Rich Text Editor)
  - `ProduktBeskrivelse` (Rich Text – shown only in modal)
  - `Pris` (Decimal)
  - `Produktbillede` (Media Picker)
  - `Produktbillede1` (Optional second Media Picker)

- `Produktside`
  - `Sidetitel` (Text)
  - Uses **child nodes of type `Produkt`** to dynamically list products

- `KontaktSide`
  - `Sidetitel`, `Beskrivelse`, `Email`, `Telefonnummer`, `Adresse`, `Kort` (Google Maps iframe)

- `HomePage`
  - `Title`, `Beskrivelse`

---

### 2. Frontend (Tailwind CSS)

- Responsive **grid layout** using Tailwind: `grid-cols-2`, `grid-cols-3`, `auto-fit`, `minmax(...)`
- Product cards designed as **Partial Views** with image, name, price, and short description
- Modal built with **Alpine.js** for interactive preview with image thumbnails, zoom, and transitions
- **Hover effects**, **mobile-first layout**, and clean design

---

### 3. Extra Features

- Modal supports multiple images with click-to-zoom preview
- Embedded Google Maps iframe on contact page
- Sticky footer and responsive navigation
- Fallbacks and validation for missing fields/images
- Fully styled contact page with SVG icons and Tailwind

---

📦 Installation og opsætning

Klon projektet:

- git clone https://github.com/nspa4921/UmbracoWebShopExample.git

- Åbn i Visual Studio / VS Code (jeg brug IntelliJ)

- Kør følgende kommandoer i terminalen (i projektroden):

- npm install
- dotnet run

Navigér til https://localhost:portnummer (port fremgår af terminalen ved start)

📊 Git-kommandoer jeg har brugt

- git init
- git add .
- git commit -m "Commit.."
- git remote add origin https://github.com/nspa4921/UmbracoWebShopExample.git
- git push -u origin main




