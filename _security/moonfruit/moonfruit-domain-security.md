---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moonfruit.com
  spf: true
hosts:
- cert_expires: Aug 27 23:29:27 2026 GMT
  host: moonfruit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moonfruit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoonFruit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MoonFruit
provider_slug: moonfruit
slug: moonfruit-domain-security
source_filename: moonfruit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moonfruit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:29:27 2026 GMT\n  hsts: false\ndomains:\n- domain: moonfruit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonfruit/refs/heads/main/security/moonfruit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Directory
- Marketing Agencies
- Digital Marketing
- Marketplace
- Website
---
