---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: peco.com
  spf: true
- caa:
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  - 0 issuewild "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apple.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.peco.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: secure.peco.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 19:28:09 2026 GMT
  host: apps.apple.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peco Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PECO Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PECO Energy
provider_slug: peco-energy
slug: peco-energy-domain-security
source_filename: peco-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: secure.peco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: apps.apple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:28:09 2026 GMT\n  hsts: null\ndomains:\n- domain: peco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apple.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  - 0 issuewild \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peco-energy/refs/heads/main/security/peco-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Electric
- Energy
- Exelon
- Mobile App
- Natural Gas
- Pennsylvania
- Smart Meter
- Utility
---
