---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ionispharma.com
  spf: true
hosts:
- cert_expires: Dec 20 01:21:05 2026 GMT
  host: www.ionispharma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.ionispharma.com
  https: false
- host: api.ionispharma.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ionis Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ionis Pharmaceuticals, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ionis Pharmaceuticals
provider_slug: ionis-pharmaceuticals
slug: ionis-pharmaceuticals-domain-security
source_filename: ionis-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ionispharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 01:21:05 2026 GMT\n  hsts: null\n- host: developer.ionispharma.com\n  https: false\n- host: api.ionispharma.com\n  https: false\ndomains:\n- domain: ionispharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ionis-pharmaceuticals/refs/heads/main/security/ionis-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3
tags:
- Pharmaceuticals
- Biotech
- RNA
---
