---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: capterra.com
  spf: true
hosts:
- cert_expires: Oct  9 16:40:38 2026 GMT
  host: www.capterra.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capterra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capterra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Capterra
provider_slug: capterra
slug: capterra-domain-security
source_filename: capterra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.capterra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:40:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: capterra.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capterra/refs/heads/main/security/capterra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- B2B
- Click Reporting
- Gartner Digital Markets
- Lead Generation
- Marketplace
- PPC
- Software Advice
- Software Comparison
- Software Reviews
---
