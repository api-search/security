---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mrc-global.com
  spf: false
hosts:
- cert_expires: Oct  7 16:29:37 2026 GMT
  host: www.mrc-global.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mrc Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MRC Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MRC Global
provider_slug: mrc-global
slug: mrc-global-domain-security
source_filename: mrc-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mrc-global.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:29:37 2026 GMT\n  hsts: null\ndomains:\n- domain: mrc-global.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mrc-global/refs/heads/main/security/mrc-global-domain-security.yml
summary_line: TLSv1.3
tags:
- Distribution
- Energy
- Industrial
- Pipe
- Valves
- Fortune 500
---
