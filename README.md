„Please note: The official main GitHub repository is not public for security reasons.“
„Hinweis: Das offizielle Haupt-GitHub-Repository ist aus Sicherheitsgründen nicht öffentlich zugänglich.“

# 🕌 ATIB Felixdorf - Gençlik Platform

Eine moderne, vollständig ausgestattete Website für die ATIB Gemeinde Felixdorf mit umfassendem Content-Management, Event-System und Benutzerverwaltung.

## 🌟 Live Demo

**Website:** [www.atibfelixdorf.org](https://www.atibfelixdorf.org)

**Detaillierte Funktionsübersicht:** [www.atibfelixdorf.org/info](https://www.atibfelixdorf.org/info)

## 🚀 Features

### 🎯 Hauptfunktionen
- **Event-Management** - Veranstaltungen mit Anmeldesystem und E-Mail-Bestätigungen
- **Galerie-System** - Kategorisierte Foto- und Medienverwaltung
- **Team-Verwaltung** - Ansprechpartner und Rollen
- **Kontakt-System** - Nachrichten mit automatischen E-Mail-Benachrichtigungen
- **News-Bereich** - Aktuelle Mitteilungen und Ankündigungen
- **Shop-System** - Produktkatalog und Bestellverwaltung

### 👥 Benutzerrollen & Berechtigungen
- **Admin** - Vollzugriff auf alle Verwaltungsfunktionen
- **Lehrer** - Stundenplan-Management und Nachrichtenverwaltung
- **Schüler** - Stundenplan-Einsicht und Nachrichten
- **Mitglieder** - Grundfunktionen und Event-Anmeldungen

### 🛠️ Admin-Features
- **Dashboard** - Übersicht über Statistiken und Aktivitäten
- **Mail-System** - SMTP/IMAP Integration für professionelle E-Mail-Kommunikation
- **Benutzer-Management** - Rollen, Berechtigungen und Benutzerdaten
- **Settings-Management** - Dynamische Konfiguration ohne Code-Änderungen
- **Statistiken** - Detaillierte Auswertungen und Reports
- **Stundenplan-System** - Für Religionsunterricht und Kurse
- **Bug-Report-System** - Benutzerfeedback und Fehlerbericht
- **Event-Management** - Veranstaltungen mit Anmeldesystem und E-Mail-Bestätigungen
- **Galerie-System** - Kategorisierte Foto- und Medienverwaltung
- **Team-Verwaltung** - Ansprechpartner und Rollen
- **Kontakt-System** - Nachrichten mit automatischen E-Mail-Benachrichtigungen
- **News-Bereich** - Aktuelle Mitteilungen und Ankündigungen
- **Shop-System** - Produktkatalog und Bestellverwaltung
- **Schüler-Management** - Benutzerdaten und Anmeldungen


### 🎨 Design & UX
- **Responsive Design** - Optimiert für Desktop, Tablet und Mobile
- **Dark/Light Mode** - Automatische Theme-Umschaltung
- **Mehrsprachigkeit** - Google Translate Integration
- **Modern UI** - Radix UI Components mit Tailwind CSS
- **Accessibility** - WCAG-konforme Bedienbarkeit

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
