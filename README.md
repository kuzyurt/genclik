„Please note: The official main GitHub repository is not public for security reasons.“
„Hinweis: Das offizielle Haupt-GitHub-Repository ist aus Sicherheitsgründen nicht öffentlich zugänglich.“

# 🕌 ATIB Felixdorf - Gençlik Platform

Eine moderne, vollständig ausgestattete Website für die ATIB Gemeinde Felixdorf mit umfassendem Content-Management, Event-System und Benutzerverwaltung.

## 🌟 Live Demo

**Website:** [www.atibfelixdorf.org](https://www.atibfelixdorf.org)

**Detaillierte Funktionsübersicht:** [www.atibfelixdorf.org/info](https://www.atibfelixdorf.org/info)

# ATIB Felixdorf Website

Dies ist das offizielle Repository für die **[ATIB Felixdorf](https://www.atibfelixdorf.org/)**.  
Die Website wurde mit **React** + **Next.js**, **Prisma** und **PostgreSQL** entwickelt.  
Sie dient als zentrale Plattform für Veranstaltungen, Galerie, Team-Übersicht, Shop-Informationen und die interne Verwaltung der Moschee.

---

## 🌐 Öffentliche Bereiche

### 🏠 Startseite (`/`)
- Übersicht über aktuelle Veranstaltungen, Galerie-Vorschau und Team-Vorschau.
- Komponenten für **Events**, **Galerie** und **Team**.

### 📅 Veranstaltungen (`/events`)
- Alle Veranstaltungen mit Kategorien.
- Möglichkeit zur Anmeldung durch Eingabe von:
  - E-Mail-Adresse, Name (Pflichtfelder)
  - Adresse, Telefonnummer, Alter (optional)
- Nach der Anmeldung erhalten Nutzer eine Bestätigungsmail von `info@atibfelixdorf.org` (angenommen/abgelehnt).

### 🖼️ Galerie (`/gallery`)
- Bildergalerie mit Kategorien (Events, Allgemein, etc.).
- Möglichkeit, einzelne Bilder in **Vollansicht** zu betrachten.

### ℹ️ Über uns (`/Über uns`)
- Mehrere Abschnitte mit Bildern zur Erklärung der Moschee.
- Dynamisch erweiterbar (über das Admin-Interface).
- Unterhalb: Teamübersicht mit Kategorien und Mitgliedern (inkl. Bild & Infos).

### 🛒 Shop (`/shop`)
- Produkte in Kategorien mit Bildern, Beschreibung & Preis.
- Beim Anklicken erscheint eine größere Ansicht.
- **Hinweis:** Derzeit kein Online-Kauf möglich – nur Info, dass das Produkt im Shop erhältlich ist.

### 📩 Kontakt (`/kontakt`)
- Formular zum Versenden von Nachrichten direkt an den Admin.

### ℹ️ Info (`/info`)
- Allgemeine Informationen über die Website.

### 🌗 Header-Funktionen
- **Tag/Nacht-Modus**
- **Sprachoptionen:** Deutsch, Englisch, Türkisch (Google Translate integriert, weitere Sprachen möglich)
- **Login/Sign-Up oder Profilanzeige** (abhängig vom Status)

---

## 👥 Benutzerrollen & Funktionen

- **Mitglied**: Profilansicht & Bearbeitung, Status (aktiv/inaktiv).
- **Schüler**: Profil + Stundenplan & Mailansicht.
- **Lehrer**: Profil + Lehrermenü (Stundenplan bearbeiten, Mails verwalten, Mails senden).
- **Mitarbeiter**: Wie Admin, aber ggf. eingeschränkte Rechte.
- **Admin**: Voller Zugriff auf Admin-Dashboard.

---

## 🛠️ Admin-Interface (`/admin/`)

Das Admin-Panel besteht aus **13 Bereichen** mit dynamischen Berechtigungen je nach User-Rolle.  
Das Layout enthält eine Seitenleiste, Admin-Header (Sprache, Dark/Light-Mode, Passwort ändern, Link zur öffentlichen Seite).

### 📋 Bereiche im Überblick

1. **Dashboard** (`/admin/`) – Begrüßungsseite  
2. **Events** – Kategorien & Events erstellen, Anmeldungen annehmen/ablehnen  
3. **Galerie** – Kategorien & Bildblöcke/Einzelbilder verwalten  
4. **Team** – Kategorien & Teammitglieder hinzufügen  
5. **Lehrermenü** – Stundenpläne erstellen/bearbeiten, Pausen einfügen, Mails verwalten  
6. **User-Management** – Nutzer bearbeiten, sperren, Mails an einzelne Nutzer oder Rollen senden (DB-gespeichert & per E-Mail versendet)  
7. **Benutzer** – Kategorien & Subkategorien (Klassen) erstellen, Schüler & Eltern verwalten, PDF-Listen generieren  
8. **Statistiken** – Events, Nutzer, Schüler, Galerie-Nutzung, Website-Zugriffe  
9. **Einstellungen**  
   - Website-Bereiche aktivieren/deaktivieren  
   - Systemstatus abrufen  
   - Inhalte von `/Über uns` verwalten  
   - Berechtigungen für Admin-Bereiche setzen  
   - Social Media Links, Impressum, AI-Modelle für Chatbot verwalten  
10. **Kontakt** – Kontaktinformationen ändern  
11. **Mails** –  
   1. Kontakt-Nachrichten ansehen & beantworten  
   2. Veranstaltungsanmeldungen verwalten  
   3. Externe Nachrichten (z. B. an `info@atibfelixdorf.org`)  
12. **News** – News-Artikel hinzufügen, bearbeiten, löschen  
13. **Bugs/Ideen** – Fehler melden, Ideen einreichen, Priorität setzen & Status verwalten  

---

## 🛠️ Tech Stack

### Frontend
- **Next.js 15** - React Framework mit App Router
- **React 18** - Moderne React Features und Hooks
- **TypeScript** - Type-safe Development
- **Tailwind CSS** - Utility-first CSS Framework
- **Radix UI** - Accessible Component Library
- **Lucide React** - Beautiful Icon Library

### Backend & Database
- **Next.js API Routes** - Serverless Backend Functions
- **Prisma ORM** - Type-safe Database Access
- **PostgreSQL** - Robust Relational Database
- **Supabase** - Authentication & Real-time Features

### Services & Integrations
- **Nodemailer** - SMTP E-Mail Versand
- **IMAP** - E-Mail Import und Synchronisation
- **Spline 3D** - Interactive 3D Graphics
- **Recharts** - Data Visualization
- **Zod** - Schema Validation

### Development & Deployment
- **ESLint** - Code Quality
- **Prettier** - Code Formatting
- **Git** - Version Control
- **Vercel** - Deployment Platform

## 📁 Projektstruktur

```
├── app/                    # Next.js App Router
│   ├── admin/             # Admin Interface
│   ├── api/               # API Routes
│   ├── auth/              # Authentication Pages
│   └── [pages]/           # Public Pages
├── components/            # React Components
│   ├── ui/                # Reusable UI Components
│   ├── admin/             # Admin-specific Components
│   └── auth/              # Authentication Components
├── lib/                   # Utility Libraries
│   ├── prisma.ts          # Database Client
│   ├── auth.tsx           # Authentication Logic
│   └── permissions.ts     # Access Control
├── prisma/                # Database Schema
├── public/                # Static Assets
└── docs/                  # Documentation
```

## 📖 Dokumentation

- **[Funktionsübersicht](https://www.atibfelixdorf.org/info)** - Detaillierte Erklärung aller Features
- **[E-Mail Konfiguration](docs/EMAIL_CONFIG.md)** - SMTP/IMAP Setup
- **[Admin Einstellungen](docs/ADMIN_SETTINGS_README.md)** - Verwaltungsoptionen
- **[Technische Details](docs/technical-information-README.md)** - Architektur und APIs

## 🔐 Sicherheit

- **Supabase Authentication** - Sichere Benutzeranmeldung
- **Role-based Access Control** - Granulare Berechtigungen
- **Input Validation** - Zod Schema Validation
- **SQL Injection Protection** - Prisma ORM
- **XSS Protection** - DOMPurify Sanitization

## 🤝 Contributing

1. Fork das Repository
2. Feature Branch erstellen (`git checkout -b feature/amazing-feature`)
3. Changes committen (`git commit -m 'Add amazing feature'`)
4. Branch pushen (`git push origin feature/amazing-feature`)
5. Pull Request öffnen

## 📄 License

Dieses Projekt ist für die ATIB Felixdorf entwickelt.

## 📞 Support

- **Website:** [www.atibfelixdorf.org](https://www.atibfelixdorf.org)
- **Kontakt:** [www.atibfelixdorf.org/contact](https://www.atibfelixdorf.org/contact)
- **Funktionen:** [www.atibfelixdorf.org/info](https://www.atibfelixdorf.org/info)

---

**Entwickelt mit ❤️ für  ATIB Felixdorf von der Atib Felixdorf Jugend**
