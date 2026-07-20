---
api_specs:
- filename: appzen-autonomous-ap-openapi-original.yml
  format: yaml
  label: Autonomous AP API
  slug: autonomous-ap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/openapi/appzen-autonomous-ap-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "trust-provider.com"
  - 0 issuewild "usertrust.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appzen.com
  spf: true
hosts:
- cert_expires: Sep 14 12:16:24 2026 GMT
  host: appzen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appzen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppZen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AppZen
provider_slug: appzen
slug: appzen-domain-security
source_filename: appzen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appzen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:16:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appzen.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"trust-provider.com\"\n  - 0 issuewild \"usertrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appzen/refs/heads/main/security/appzen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Accounts Payable
- Expense Management
- Invoice Processing
- Spend Audit
- Artificial Intelligence
- ERP Integration
---
