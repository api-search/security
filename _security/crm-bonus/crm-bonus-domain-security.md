---
api_specs:
- filename: crm-bonus-oto-data-api-openapi.yml
  format: yaml
  label: Oto Data API
  slug: oto-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/openapi/crm-bonus-oto-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crmbonus.com.br
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: otocrm.com.br
  spf: true
hosts:
- cert_expires: Oct 15 14:32:16 2026 GMT
  host: crmbonus.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 02:20:41 2026 GMT
  host: data-api.otocrm.com.br
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: 'Corrected by hand after the automated pass recorded hsts: null. The probe''s request path returns 404 on this host and the header was missed; a live HEAD on https://data-api.otocrm.com.br/ and on /docs both return "strict-transport-security: max-age=31536000; includeSubDomains" (re-verified 2026-08-12). Fronted by Cloudflare.'
  tls_version: TLSv1.3
- cert_expires: Oct 23 02:20:41 2026 GMT
  host: data-api-hmg.otocrm.com.br
  hsts: null
  https: true
  note: staging (homologação) host; HSTS not confirmed.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crm Bonus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CRM Bonus, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CRM Bonus
provider_slug: crm-bonus
slug: crm-bonus-domain-security
source_filename: crm-bonus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crmbonus.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:32:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data-api.otocrm.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 02:20:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Corrected by hand after the automated pass recorded hsts: null. The probe's\n    request path returns 404 on this host and the header was missed; a live\n    HEAD on https://data-api.otocrm.com.br/ and on /docs both return\n    \"strict-transport-security: max-age=31536000; includeSubDomains\"\n    (re-verified 2026-08-12). Fronted by Cloudflare.\n- host: data-api-hmg.otocrm.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 02:20:41 2026 GMT\n  hsts: null\n  note: staging (homologação) host; HSTS not confirmed.\n\
  domains:\n- domain: crmbonus.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: otocrm.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crm-bonus/refs/heads/main/security/crm-bonus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Loyalty
- Cashback
- CRM
- Retail Media
- E-Commerce
- Brazil
- WhatsApp
- Customer Data
- Data Ingestion
- Point-of-Sale
---
