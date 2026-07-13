---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com; account=97d8cb21ded856f534dc92b1c92f5916fa401221a6e28bf2d05e743d2fdb2455"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: questdiagnostics.com
  spf: true
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: www.questdiagnostics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Quest Diagnostics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quest Diagnostics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quest Diagnostics
provider_slug: quest-diagnostics
slug: quest-diagnostics-domain-security
source_filename: quest-diagnostics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.questdiagnostics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: questdiagnostics.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com; account=97d8cb21ded856f534dc92b1c92f5916fa401221a6e28bf2d05e743d2fdb2455\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quest-diagnostics/refs/heads/main/security/quest-diagnostics-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Diagnostics
- Fortune 500
- Healthcare
- Laboratory
- Lab Services
---
