---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fontawesome.com
  spf: true
hosts:
- cert_expires: Sep 12 23:11:14 2026 GMT
  host: docs.fontawesome.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 23:11:14 2026 GMT
  host: api.fontawesome.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Font Awesome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Font Awesome, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Font Awesome
provider_slug: font-awesome
slug: font-awesome-domain-security
source_filename: font-awesome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.fontawesome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:11:14 2026 GMT\n  hsts: false\n- host: api.fontawesome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:11:14 2026 GMT\n  hsts: null\ndomains:\n- domain: fontawesome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/font-awesome/refs/heads/main/security/font-awesome-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Icons
- SVG
- Fonts
- Web Design
- Developer Tools
- GraphQL
- Icon Library
- Frontend
- Design System
- Company
---
