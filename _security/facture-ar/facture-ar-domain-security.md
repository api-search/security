---
api_specs:
- filename: facture-ar-borradores-api-openapi.yml
  format: yaml
  label: Facturear Borradores API
  slug: facture-ar-borradores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-borradores-api-openapi.yml
- filename: facture-ar-cuits-api-openapi.yml
  format: yaml
  label: Facturear CUITs API
  slug: facture-ar-cuits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-cuits-api-openapi.yml
- filename: facture-ar-facturas-api-openapi.yml
  format: yaml
  label: Facturear Facturas API
  slug: facture-ar-facturas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-facturas-api-openapi.yml
- filename: facture-ar-importar-desde-arca-api-openapi.yml
  format: yaml
  label: Facturear Importar desde ARCA API
  slug: facture-ar-importar-desde-arca-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-importar-desde-arca-api-openapi.yml
- filename: facture-ar-lotes-api-openapi.yml
  format: yaml
  label: Facturear Lotes API
  slug: facture-ar-lotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-lotes-api-openapi.yml
- filename: facture-ar-plantillas-api-openapi.yml
  format: yaml
  label: Facturear Plantillas API
  slug: facture-ar-plantillas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-plantillas-api-openapi.yml
- filename: facture-ar-reportes-api-openapi.yml
  format: yaml
  label: Facturear Reportes API
  slug: facture-ar-reportes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-reportes-api-openapi.yml
- filename: facture-ar-utilidades-api-openapi.yml
  format: yaml
  label: Facturear Utilidades API
  slug: facture-ar-utilidades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-utilidades-api-openapi.yml
- filename: facture-ar-webhooks-api-openapi.yml
  format: yaml
  label: Facturear Webhooks API
  slug: facture-ar-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facture-ar/openapi/facture-ar-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: facture.ar
  spf: true
hosts:
- cert_expires: Dec 29 10:41:07 2026 GMT
  host: facture.ar
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Facturear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facturear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Facturear
provider_slug: facture-ar
slug: facture-ar-domain-security
source_filename: facture-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: facture.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 10:41:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: facture.ar\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/facture-ar/security/facture-ar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Invoicing
- Argentina
- Software-as-a-Service
---
