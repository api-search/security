---
api_specs:
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Jobs API
  slug: bigchange-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Contacts and Persons API
  slug: bigchange-contacts-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Finance API
  slug: bigchange-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Stock and Inventory API
  slug: bigchange-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Resources, Users and Vehicles API
  slug: bigchange-resources-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Notes and Worksheets API
  slug: bigchange-notes-worksheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: bigchange-openapi.yml
  format: yaml
  label: BigChange Reference Data API
  slug: bigchange-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/openapi/bigchange-openapi.yml
- filename: swagger.json
  format: json
  label: BigChange Asset Management API
  slug: bigchange-asset-management-api
  spec_type: OpenAPI
  url: https://api.bigchange.com/swagger/asset-management/v1/swagger.json
- filename: swagger.json
  format: json
  label: BigChange Webhooks API
  slug: bigchange-webhooks-api
  spec_type: OpenAPI
  url: https://api.bigchange.com/swagger/webhooks/v1/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; pct=100; rua=mailto:92gbf4jq@ag.eu.dmarcian.com;
  dnssec: false
  domain: bigchange.com
  spf: true
  spf_record: v=spf1 include:amazonses.com include:_spf.google.com include:spf.us.exclaimer.net include:spf.hubspotemail.net include:_spf.salesforce.com include:spf.bigchange.com ip4:167.89.0.0/17 ip4:149.72.0.0/16 ip4:159.183.0.0/16 ~all
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  cert_issuer: Amazon RSA 2048 M02
  cert_starts: Aug 12 00:00:00 2025 GMT
  cert_subject: CN=api.bigchange.com
  host: api.bigchange.com
  hsts: false
  https: true
  note: Root returns HTTP 403 (WAF/allowlisted); API paths respond. openssl handshake blocked, cert captured via curl.
  tls_version: TLSv1.3
- cert_expires: Oct  2 13:50:44 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  cert_starts: Jul  4 12:50:54 2026 GMT
  cert_subject: CN=bigchange.com
  host: bigchange.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developers.bigchange.com
  hsts: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: Developer portal enforces HSTS with includeSubDomains and preload.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bigchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BigChange, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BigChange
provider_slug: bigchange
slug: bigchange-domain-security
source_filename: bigchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.bigchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: 'Amazon RSA 2048 M02'\n  cert_subject: 'CN=api.bigchange.com'\n  cert_starts: Aug 12 00:00:00 2025 GMT\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: false\n  note: 'Root returns HTTP 403 (WAF/allowlisted); API paths respond. openssl handshake blocked, cert captured via curl.'\n- host: bigchange.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: 'Google Trust Services (WE1)'\n  cert_subject: 'CN=bigchange.com'\n  cert_starts: Jul  4 12:50:54 2026 GMT\n  cert_expires: Oct  2 13:50:44 2026 GMT\n  hsts: false\n- host: developers.bigchange.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_preload: true\n  note: 'Developer portal enforces HSTS with includeSubDomains and preload.'\ndomains:\n- domain: bigchange.com\n  dnssec: false\n  caa:\
  \ []\n  spf: true\n  spf_record: 'v=spf1 include:amazonses.com include:_spf.google.com include:spf.us.exclaimer.net include:spf.hubspotemail.net include:_spf.salesforce.com include:spf.bigchange.com ip4:167.89.0.0/17 ip4:149.72.0.0/16 ip4:159.183.0.0/16 ~all'\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_pct: 100\n  dmarc_record: 'v=DMARC1; p=reject; pct=100; rua=mailto:92gbf4jq@ag.eu.dmarcian.com;'\nnotes: >-\n  Live probes on 2026-07-12. Email authentication is strong on the apex domain\n  (SPF present, DMARC at p=reject/100%). No CAA records published and DNSSEC not\n  enabled (AD flag absent; NS on AWS Route 53). HSTS is enforced on the developer\n  portal but was not observed on api.bigchange.com or the apex www host at probe\n  time.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigchange/refs/heads/main/security/bigchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service Management
- Job Management
- Scheduling
- Workforce Management
- Fleet
- CRM
- SaaS
---
