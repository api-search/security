---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brightfunds.org
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: www.brightfunds.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bright Funds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright Funds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bright Funds
provider_slug: bright-funds
slug: bright-funds-domain-security
source_filename: bright-funds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightfunds.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brightfunds.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-funds/refs/heads/main/security/bright-funds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Workplace Giving
- Corporate Social Responsibility
- Employee Engagement
- Nonprofits
- Grants Management
- Donations
- Volunteering
- OAuth
- OpenID Connect
---
