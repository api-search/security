---
api_specs:
- filename: mioffice-ai-catalog-api-openapi.yml
  format: yaml
  label: MiOffice AI Catalog API
  slug: mioffice-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mioffice-ai/openapi/mioffice-ai-catalog-api-openapi.yml
- filename: mioffice-ai-copilot-api-openapi.yml
  format: yaml
  label: MiOffice AI Copilot API
  slug: mioffice-ai-copilot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mioffice-ai/openapi/mioffice-ai-copilot-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mioffice.ai
  spf: true
hosts:
- cert_expires: Jan  4 22:27:45 2027 GMT
  host: mioffice.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MiOffice AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MiOffice AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MiOffice AI
provider_slug: mioffice-ai
slug: mioffice-ai-domain-security
source_filename: mioffice-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mioffice.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 22:27:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mioffice.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mioffice-ai/security/mioffice-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Workspace
- Collaboration
- Document Processing
- Media
---
