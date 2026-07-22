---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: finleycms.com
  spf: true
hosts:
- cert_expires: Oct  4 05:36:47 2026 GMT
  host: www.finleycms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finley Concord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finley (Concord), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Finley (Concord)
provider_slug: finley-concord
slug: finley-concord-domain-security
source_filename: finley-concord-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finleycms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:36:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: finleycms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finley-concord/refs/heads/main/security/finley-concord-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- Fintech
- Loan Servicing
- Loan Administration
- Debt Capital Markets
- Private Credit
- Portfolio Monitoring
---
