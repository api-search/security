---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: televisaunivision.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vix.com
  spf: true
hosts:
- cert_expires: Sep  8 17:17:52 2026 GMT
  host: corporate.televisaunivision.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 16:05:18 2026 GMT
  host: vix.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: www.uforia.com
  https: false
kind: domain-security
layout: security
method: probed
name: Univision Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TelevisaUnivision (Univision Communications), probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TelevisaUnivision (Univision Communications)
provider_slug: univision-communications
slug: univision-communications-domain-security
source_filename: univision-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corporate.televisaunivision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 17:17:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 16:05:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.uforia.com\n  https: false\ndomains:\n- domain: televisaunivision.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: vix.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/univision-communications/refs/heads/main/security/univision-communications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media
- Streaming
- Hispanic
- Advertising
- Television
- Radio
- Content
---
