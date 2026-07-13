---
api_specs:
- filename: ada-knowledge-openapi.yml
  format: yaml
  label: Ada Knowledge API
  slug: ada-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-knowledge-openapi.yml
- filename: ada-data-export-openapi.yml
  format: yaml
  label: Ada Data Export API
  slug: ada-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-data-export-openapi.yml
- filename: ada-data-compliance-openapi.yml
  format: yaml
  label: Ada Data Compliance API
  slug: ada-data-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-data-compliance-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ada.cx
  spf: true
hosts:
- cert_expires: Aug 21 19:01:27 2026 GMT
  host: www.ada.cx
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 16:41:43 2026 GMT
  host: docs.ada.cx
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.ada.cx
  https: false
kind: domain-security
layout: security
method: probed
name: Ada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ada, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ada
provider_slug: ada
slug: ada-domain-security
source_filename: ada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ada.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:01:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.ada.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 16:41:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ada.cx\n  https: false\ndomains:\n- domain: ada.cx\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/security/ada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ai
- customer-service
- chatbot
- automation
- conversational-ai
- helpdesk
- crm
- integrations
- knowledge-management
- data-export
---
