---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: corpay.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: www.corpay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fleetcor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corpay (formerly FLEETCOR), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Corpay (formerly FLEETCOR)
provider_slug: fleetcor
slug: fleetcor-domain-security
source_filename: fleetcor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: corpay.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleetcor/refs/heads/main/security/fleetcor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B Payments
- Corporate Payments
- Fleet Cards
- Fuel Cards
- Commercial Cards
- AP Automation
- Accounts Payable
- Cross-Border Payments
- Foreign Exchange
- Lodging
- Expense Management
- ERP Integration
---
