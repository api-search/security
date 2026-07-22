---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ventasreit.com
  spf: true
hosts:
- cert_expires: Sep 24 14:48:14 2026 GMT
  host: www.ventasreit.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ventas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ventas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ventas
provider_slug: ventas
slug: ventas-domain-security
source_filename: ventas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ventasreit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 14:48:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: ventasreit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ventas/refs/heads/main/security/ventas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Real Estate
- REIT
- Senior Housing
- Life Science
- Fortune 500
---
