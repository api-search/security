---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 88rising.com
  spf: true
hosts:
- cert_expires: Oct 11 23:48:12 2026 GMT
  host: 88rising.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 88Rising Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 88rising, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 88rising
provider_slug: 88rising
slug: 88rising-domain-security
source_filename: 88rising-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 88rising.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:48:12 2026 GMT\n  hsts: false\ndomains:\n- domain: 88rising.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/88rising/refs/heads/main/security/88rising-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Media
- Entertainment
- Music
- Record Label
- Live Events
- Content
- Marketing
---
