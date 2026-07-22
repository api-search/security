---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: readkami.com
  spf: false
hosts:
- cert_expires: Sep  3 12:04:00 2026 GMT
  host: readkami.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kami Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KAMI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: KAMI
provider_slug: kami
slug: kami-domain-security
source_filename: kami-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: readkami.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 12:04:00 2026 GMT\n  hsts: null\ndomains:\n- domain: readkami.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kami/refs/heads/main/security/kami-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Entertainment
- Webtoons
- Comics
- Storytelling
- Consumer App
- Media
- Turkey
---
