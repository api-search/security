---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:netis@heska.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: heska.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ezyvet.com
  spf: true
hosts:
- cert_expires: Jul 28 11:35:17 2026 GMT
  host: www.heska.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 14:39:58 2026 GMT
  host: docs.ezyvet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 12:51:04 2026 GMT
  host: careville.instinct.vet
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heska Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heska, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Heska
provider_slug: heska
slug: heska-domain-security
source_filename: heska-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heska.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 11:35:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ezyvet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:39:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: careville.instinct.vet\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 12:51:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heska.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:netis@heska.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ezyvet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heska/refs/heads/main/security/heska-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Veterinary
- Diagnostics
- Animal Health
- Point of Care
- Lab Analyzers
- Partner API
- Antech
- Mars
---
