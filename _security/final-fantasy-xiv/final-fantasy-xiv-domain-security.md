---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xivapi.com
  spf: false
hosts:
- cert_expires: Aug 18 21:57:20 2026 GMT
  host: xivapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Final Fantasy Xiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Final Fantasy XIV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Final Fantasy XIV
provider_slug: final-fantasy-xiv
slug: final-fantasy-xiv-domain-security
source_filename: final-fantasy-xiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xivapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 21:57:20 2026 GMT\n  hsts: false\ndomains:\n- domain: xivapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/final-fantasy-xiv/refs/heads/main/security/final-fantasy-xiv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Games And Comics
- Public APIs
---
