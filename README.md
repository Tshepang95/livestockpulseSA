livestockpulse/
│
├── README.md
├── LICENSE
├── .gitignore
├── .env.example
├── package.json
├── netlify.toml
│
├── index.html
├── 404.html
│
├── public/
│   ├── robots.txt
│   ├── sitemap.xml
│   ├── manifest.json
│   ├── favicon.ico
│   └── favicon.svg
│
├── src/
│   ├── assets/
│   │   ├── images/
│   │   │   ├── hero/
│   │   │   │   ├── livestockpulse-device-front.png
│   │   │   │   ├── livestockpulse-device-angle.png
│   │   │   │   ├── livestockpulse-device-back.png
│   │   │   │   └── device-scan-demo.mp4
│   │   │   │
│   │   │   ├── illustrations/
│   │   │   │   ├── blockchain-verification.svg
│   │   │   │   ├── qr-scan-process.svg
│   │   │   │   ├── gps-tracking.svg
│   │   │   │   └── outbreak-map.svg
│   │   │   │
│   │   │   ├── icons/
│   │   │   │   ├── cattle-outline.svg
│   │   │   │   ├── vet-badge.svg
│   │   │   │   ├── blockchain-icon.svg
│   │   │   │   ├── shield-check.svg
│   │   │   │   ├── alert-triangle.svg
│   │   │   │   └── government-building.svg
│   │   │   │
│   │   │   └── team/
│   │   │       ├── tshepang-masilo.jpg
│   │   │       └── tech-unicorns-logo.svg
│   │   │
│   │   └── fonts/
│   │       ├── inter-regular.woff2
│   │       ├── inter-bold.woff2
│   │       └── inter-extrabold.woff2
│   │
│   ├── css/
│   │   ├── main.css
│   │   ├── components.css
│   │   ├── pages/
│   │   │   ├── home.css
│   │   │   ├── dashboard.css
│   │   │   ├── scanner.css
│   │   │   ├── admin.css
│   │   │   └── auth.css
│   │   │
│   │   └── vendors/
│   │       ├── chartjs.css
│   │       └── leaflet.css
│   │
│   ├── js/
│   │   ├── main.js
│   │   ├── router.js
│   │   ├── config.js
│   │   │
│   │   ├── core/
│   │   │   ├── auth.js
│   │   │   ├── api.js
│   │   │   ├── blockchain.js
│   │   │   ├── qr-generator.js
│   │   │   ├── qr-scanner.js
│   │   │   ├── gps-tracker.js
│   │   │   ├── offline-storage.js
│   │   │   └── error-handler.js
│   │   │
│   │   ├── services/
│   │   │   ├── animal-service.js
│   │   │   ├── user-service.js
│   │   │   ├── outbreak-service.js
│   │   │   ├── export-service.js
│   │   │   └── notification-service.js
│   │   │
│   │   ├── components/
│   │   │   ├── navbar.js
│   │   │   ├── sidebar.js
│   │   │   ├── charts/
│   │   │   │   ├── outbreak-chart.js
│   │   │   │   ├── roi-chart.js
│   │   │   │   └── movement-chart.js
│   │   │   │
│   │   │   ├── maps/
│   │   │   │   ├── outbreak-map.js
│   │   │   │   ├── heatmap-layer.js
│   │   │   │   └── quarantine-zone.js
│   │   │   │
│   │   │   └── tables/
│   │   │       ├── animal-table.js
│   │   │       └── audit-table.js
│   │   │
│   │   ├── pages/
│   │   │   ├── home.js
│   │   │   ├── dashboard.js
│   │   │   ├── scanner.js
│   │   │   ├── reports.js
│   │   │   └── settings.js
│   │   │
│   │   └── utils/
│   │       ├── validators.js
│   │       ├── formatters.js
│   │       ├── permissions.js
│   │       ├── constants.js
│   │       └── helpers.js
│   │
│   └── pages/
│       ├── home.html
│       ├── dashboard.html
│       ├── scanner.html
│       ├── reports.html
│       ├── admin.html
│       ├── login.html
│       ├── register.html
│       ├── forgot-password.html
│       └── privacy-policy.html
│
├── netlify/
│   └── functions/
│       ├── auth/
│       │   ├── login.js
│       │   ├── register.js
│       │   ├── verify.js
│       │   └── logout.js
│       │
│       ├── animals/
│       │   ├── create.js
│       │   ├── read.js
│       │   ├── update.js
│       │   ├── delete.js
│       │   ├── list.js
│       │   ├── search.js
│       │   ├── movements.js
│       │   └── health-records.js
│       │
│       ├── blockchain/
│       │   ├── verify-hash.js
│       │   ├── write-record.js
│       │   ├── read-record.js
│       │   └── batch-verify.js
│       │
│       ├── qr/
│       │   ├── generate.js
│       │   ├── validate.js
│       │   └── decode.js
│       │
│       ├── outbreaks/
│       │   ├── report.js
│       │   ├── trace.js
│       │   ├── quarantine.js
│       │   ├── alerts.js
│       │   └── heatmap.js
│       │
│       ├── users/
│       │   ├── profile.js
│       │   ├── roles.js
│       │   ├── permissions.js
│       │   └── activity-log.js
│       │
│       ├── exports/
│       │   ├── generate-report.js
│       │   ├── export-csv.js
│       │   └── export-pdf.js
│       │
│       ├── notifications/
│       │   ├── send-alert.js
│       │   ├── sms.js
│       │   └── email.js
│       │
│       ├── hardware/
│       │   ├── register-device.js
│       │   ├── sync-data.js
│       │   ├── verify-device.js
│       │   └── device-status.js
│       │
│       ├── webhooks/
│       │   ├── blockchain-webhook.js
│       │   └── sms-webhook.js
│       │
│       └── utils/
│           ├── supabase-client.js
│           ├── blockchain-client.js
│           ├── validation.js
│           ├── rate-limiter.js
│           └── logger.js
│
├── supabase/
│   ├── migrations/
│   │   ├── 001_initial_schema.sql
│   │   ├── 002_rls_policies.sql
│   │   ├── 003_functions.sql
│   │   ├── 004_triggers.sql
│   │   └── 005_seed_data.sql
│   │
│   ├── seeds/
│   │   ├── roles.sql
│   │   ├── users.sql
│   │   └── demo-animals.sql
│   │
│   └── types/
│       └── database.types.ts
│
├── blockchain/
│   ├── contracts/
│   │   ├── AnimalHealthRecord.sol
│   │   ├── MovementPermit.sol
│   │   ├── RoleManager.sol
│   │   └── interfaces/
│   │       └── IAnimalHealth.sol
│   │
│   ├── scripts/
│   │   ├── deploy.js
│   │   ├── verify.js
│   │   └── interact.js
│   │
│   └── test/
│       ├── AnimalHealth.test.js
│       └── MovementPermit.test.js
│
├── tests/
│   ├── unit/
│   │   ├── auth.test.js
│   │   ├── blockchain.test.js
│   │   └── validators.test.js
│   │
│   ├── integration/
│   │   ├── api.test.js
│   │   └── database.test.js
│   │
│   └── e2e/
│       └── scanner-flow.test.js
│
├── docs/
│   ├── api/
│   │   ├── README.md
│   │   ├── authentication.md
│   │   ├── animals.md
│   │   ├── blockchain.md
│   │   └── webhooks.md
│   │
│   ├── architecture/
│   │   ├── overview.md
│   │   ├── database-schema.md
│   │   ├── blockchain-integration.md
│   │   └── security.md
│   │
│   └── user-guides/
│       ├── farmer-guide.md
│       ├── vet-guide.md
│       └── auditor-guide.md
│
├── scripts/
│   ├── deploy.sh
│   ├── backup-db.sh
│   ├── seed-demo-data.js
│   └── generate-types.js
│
└── config/
    ├── development.js
    ├── staging.js
    ├── production.js
    └── test.js

#   l i v e s t o c k p u l s e  
 #   l i v e s t o c k p u l s e S A  
 #   l i v e s t o c k p u l s e S A  
 