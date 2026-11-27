---
api_specs:
- filename: vng-realisatie-autorisaties-openapi.yml
  format: yaml
  label: VNG Realisatie Autorisaties API
  slug: vng-realisatie-autorisaties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-autorisaties-openapi.yml
- filename: vng-realisatie-besluiten-openapi.yml
  format: yaml
  label: VNG Realisatie Besluiten API
  slug: vng-realisatie-besluiten-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-besluiten-openapi.yml
- filename: vng-realisatie-catalogi-openapi.yml
  format: yaml
  label: VNG Realisatie Catalogi API
  slug: vng-realisatie-catalogi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-catalogi-openapi.yml
- filename: vng-realisatie-documenten-openapi.yml
  format: yaml
  label: VNG Realisatie Documenten API
  slug: vng-realisatie-documenten-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-documenten-openapi.yml
- filename: vng-realisatie-klantinteracties-openapi.yml
  format: yaml
  label: VNG Realisatie Klantinteracties
  slug: vng-realisatie-klantinteracties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-klantinteracties-openapi.yml
- filename: vng-realisatie-notificaties-openapi.yml
  format: yaml
  label: VNG Realisatie Notification API
  slug: vng-realisatie-notificaties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-notificaties-openapi.yml
- filename: vng-realisatie-referentielijsten-openapi.yml
  format: yaml
  label: VNG Realisatie Referentielijsten & Selectielijst API
  slug: vng-realisatie-referentielijsten-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-referentielijsten-openapi.yml
- filename: vng-realisatie-woz-bevragen-openapi.yml
  format: yaml
  label: VNG Realisatie BG IMWOZ WOZ
  slug: vng-realisatie-woz-bevragen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-woz-bevragen-openapi.yml
- filename: vng-realisatie-zaken-openapi.yml
  format: yaml
  label: VNG Realisatie Zaken API
  slug: vng-realisatie-zaken-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vng-realisatie/openapi/vng-realisatie-zaken-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vng.nl
  spf: true
hosts:
- cert_expires: Nov 12 14:30:18 2026 GMT
  host: standaarden.vng.nl
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: VNG Realisatie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VNG Realisatie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: VNG Realisatie
provider_slug: vng-realisatie
slug: vng-realisatie-domain-security
source_filename: vng-realisatie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: standaarden.vng.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 14:30:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: vng.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/vng-realisatie/security/vng-realisatie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Municipalities
- Netherlands
- API Standards
- Common Ground
- Open Standard
- Public Sector
---
