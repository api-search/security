---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: f6s.com
  spf: true
hosts:
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: www.f6s.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 17:57:17 2026 GMT
  host: developers.f6s.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: F6S Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for F6S, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: F6S
provider_slug: f6s
slug: f6s-domain-security
source_filename: f6s-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.f6s.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: null\n- host: developers.f6s.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 17:57:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: f6s.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/f6s/refs/heads/main/security/f6s-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accelerators
- Funding
- Jobs
- Startups
---
