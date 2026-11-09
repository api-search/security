---
api_specs:
- filename: auditae-app-billing-api-openapi.yml
  format: yaml
  label: AuditAE Billing API
  slug: auditae-app-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auditae-app/openapi/auditae-app-billing-api-openapi.yml
- filename: auditae-app-citations-api-openapi.yml
  format: yaml
  label: AuditAE Citations API
  slug: auditae-app-citations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auditae-app/openapi/auditae-app-citations-api-openapi.yml
- filename: auditae-app-schema-api-openapi.yml
  format: yaml
  label: AuditAE Schema API
  slug: auditae-app-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auditae-app/openapi/auditae-app-schema-api-openapi.yml
- filename: auditae-app-technical-api-openapi.yml
  format: yaml
  label: AuditAE Technical API
  slug: auditae-app-technical-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/auditae-app/openapi/auditae-app-technical-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: auditae.app
  spf: false
hosts:
- cert_expires: Dec  5 04:35:20 2026 GMT
  host: auditae.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auditae App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AuditAE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AuditAE
provider_slug: auditae-app
slug: auditae-app-domain-security
source_filename: auditae-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auditae.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 04:35:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: auditae.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/auditae-app/security/auditae-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- SEO
- Marketing
- Software-as-a-Service
- Visibility
---
