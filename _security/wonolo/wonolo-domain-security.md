---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "  amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wonolo.com
  spf: true
hosts:
- cert_expires: Oct  5 21:24:54 2026 GMT
  host: www.wonolo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: api.wonolo.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wonolo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wonolo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wonolo
provider_slug: wonolo
slug: wonolo-domain-security
source_filename: wonolo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wonolo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:24:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wonolo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: wonolo.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"  amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wonolo/refs/heads/main/security/wonolo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Staffing
- Workforce
- Human Resources
- Marketplace
- Gig Economy
- Recruiting
- Labor
- On-Demand
---
