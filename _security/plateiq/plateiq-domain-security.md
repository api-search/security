---
api_specs:
- filename: plateiq-openapi.yaml
  format: yaml
  label: Ottimate API
  slug: ottimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/openapi/plateiq-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plateiq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ottimate.com
  spf: true
hosts:
- cert_expires: Sep 23 15:20:12 2026 GMT
  host: plateiq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 01:01:08 2026 GMT
  host: api.ottimate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 18:31:18 2026 GMT
  host: sandbox-api.ottimate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plateiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlateIQ, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PlateIQ
provider_slug: plateiq
slug: plateiq-domain-security
source_filename: plateiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plateiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:20:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ottimate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 01:01:08 2026 GMT\n  hsts: null\n- host: sandbox-api.ottimate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:31:18 2026 GMT\n  hsts: null\ndomains:\n- domain: plateiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ottimate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plateiq/refs/heads/main/security/plateiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Accounts Payable
- Invoice Automation
- Payments
- Fintech
- Restaurants
- Procurement
- Spend Management
- ERP Integration
---
