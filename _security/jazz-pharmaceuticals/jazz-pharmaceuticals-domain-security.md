---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jazzpharma.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.jazzpharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.jazzpharma.com
  https: false
- host: api.jazzpharma.com
  https: false
kind: domain-security
layout: security
method: probed
name: Jazz Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jazz Pharmaceuticals, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jazz Pharmaceuticals
provider_slug: jazz-pharmaceuticals
slug: jazz-pharmaceuticals-domain-security
source_filename: jazz-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jazzpharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\n- host: developer.jazzpharma.com\n  https: false\n- host: api.jazzpharma.com\n  https: false\ndomains:\n- domain: jazzpharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jazz-pharmaceuticals/refs/heads/main/security/jazz-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pharmaceuticals
- Neuroscience
---
