---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apogeeent.com
  spf: true
hosts:
- cert_expires: Nov 29 07:10:10 2026 GMT
  host: www.apogeeent.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apogee Interactive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apogee Interactive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Apogee Interactive
provider_slug: apogee-interactive
slug: apogee-interactive-domain-security
source_filename: apogee-interactive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apogeeent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 07:10:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: apogeeent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apogee-interactive/refs/heads/main/security/apogee-interactive-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Indie Publishing
- Game Publishing
- IP Development
- Marketing
- Developer Support
---
