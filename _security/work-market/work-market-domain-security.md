---
api_specs:
- filename: work-market-employer-api-openapi.yml
  format: yaml
  label: WorkMarket Employer API
  slug: workmarket-employer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/openapi/work-market-employer-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "digicert.com"
  - 0 issue "comodoca.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workmarket.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: workmarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 22:08:27 2026 GMT
  host: employer-api.workmarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: www.workmarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Work Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Work Market, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Work Market
provider_slug: work-market
slug: work-market-domain-security
source_filename: work-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: employer-api.workmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:08:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.workmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: workmarket.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/work-market/refs/heads/main/security/work-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Workforce Management
- Contractors
- Freelance
- Gig Economy
- Human Resources
- Payments
- Field Services
- Staffing
---
