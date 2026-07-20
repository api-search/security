---
api_specs:
- filename: boostup-openapi-original.json
  format: json
  label: Boostup Export API
  slug: boostup-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boostup/refs/heads/main/openapi/boostup-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:alerts@terret.ai"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: terret.ai
  spf: true
- caa:
  - 0 iodef "mailto:amit@boostup.ai"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: boostup.ai
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.terret.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: app.boostup.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Boostup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boostup, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Boostup
provider_slug: boostup
slug: boostup-domain-security
source_filename: boostup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.terret.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\n- host: app.boostup.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: terret.ai\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:alerts@terret.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: boostup.ai\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:amit@boostup.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boostup/refs/heads/main/security/boostup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Revenue Intelligence
- Sales
- Forecasting
- Analytics
- RevOps
- Conversation Intelligence
- Data Export
- CRM
---
