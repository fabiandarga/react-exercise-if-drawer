# Aufgabe: Conditional Rendering kennenlernen

Wir wollen eine Drawer- oder Collapsible-Komponente bauen.
Diese hat einen Titel, der immer sichtbar ist und ein body-teil, der ein- und ausgeblendet werden kann.

## Vorbereitung

```bash
npm create vite@latest aufgabe-react-drawer -- --template react-ts
cd aufgabe-react-drawer
npm install
npm run dev
```

Optional: Wähle die TypeScript-Variante

## Drawer Komponente

1. Erstelle einen neuen Ordner `/src/components`
2. Lege eine neue Datei `/src/components/Drawer.tsx` an

Tipps (nicht vergessen):

1. import { useState } from 'react'
2. Functional Component erstellen
3. useState für den State (isOpen)
4. Mit bedingtem Rendering (&&) Elemente ein-/ausblenden
5. onClick={() => funcName()} um eine Funktion auszuführen
6. Component exportieren
7. importiere und verwende die Drawer Komponente in der App.jsx

## HTML/JSX

Als Vorlage für das JSX kannst du diese Struktur benutzen:

```jsx
<div className="drawer">
    <h2>Titel</h2>
    <p>Body</p>
</div>
```

## Style

Erstelle eine Datei `/src/components/Drawer.module.css` mit folgendem Inhalt und importiere sie in der Komponente:

```css
.drawer {
    border: 1px solid #ccc;
    border-radius: 4px;
    margin: 1rem 0;
}

.drawer h2 {
    margin: 0;
    padding: 1rem;
    background: #f5f5f5;
    cursor: pointer;
    display: flex;
    justify-content: space-between;
}

.drawer p {
    padding: 1rem;
    margin: 0;
}
```

Import in der Komponente:

```tsx
import styles from "./Drawer.module.css";
```

Verwendung:

```tsx
<div className={styles.drawer}>
```
