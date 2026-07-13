---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aptiv.com
  spf: true
hosts:
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.aptiv.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: developer.aptiv.com
  https: false
- host: api.aptiv.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aptiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aptiv, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aptiv
provider_slug: aptiv
slug: aptiv-domain-security
source_filename: aptiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aptiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.aptiv.com\n  https: false\n- host: api.aptiv.com\n  https: false\ndomains:\n- domain: aptiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptiv/refs/heads/main/security/aptiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Electrical Systems
- Technology
---
