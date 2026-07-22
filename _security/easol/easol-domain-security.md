---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: easol.com
  spf: true
hosts:
- cert_expires: Sep  4 20:30:30 2026 GMT
  host: www.easol.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Easol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Easol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Easol
provider_slug: easol
slug: easol-domain-security
source_filename: easol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.easol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:30:30 2026 GMT\n  hsts: false\ndomains:\n- domain: easol.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easol/refs/heads/main/security/easol-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SaaS
- Experience Commerce
- Ticketing
- Booking
- Payments
- Events
- Travel
- CRM
---
