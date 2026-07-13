---
api_specs:
- filename: emburse-virtual-cards-openapi.yml
  format: yaml
  label: Emburse Virtual Cards API
  slug: emburse-virtual-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emburse/refs/heads/main/openapi/emburse-virtual-cards-openapi.yml
- filename: emburse-enterprise-allocation-openapi.yml
  format: yaml
  label: Emburse Enterprise REST APIs
  slug: emburse-enterprise-rest-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emburse/refs/heads/main/openapi/emburse-enterprise-allocation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: emburse.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: certify.com
  spf: true
hosts:
- cert_expires: Sep 22 22:18:59 2026 GMT
  host: www.emburse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.emburse.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:40:45 2026 GMT
  host: help.certify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emburse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emburse, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Emburse
provider_slug: emburse
slug: emburse-domain-security
source_filename: emburse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emburse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:18:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.emburse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\n- host: help.certify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:40:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: emburse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: certify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emburse/refs/heads/main/security/emburse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Expense Management
- AP Automation
- Corporate Cards
- Virtual Cards
- Receipt Capture
- Reimbursement
- Invoice Processing
- Finance
- FinTech
---
