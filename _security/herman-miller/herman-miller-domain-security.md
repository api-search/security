---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hermanmiller.com
  spf: true
hosts:
- cert_expires: Oct  1 19:27:32 2026 GMT
  host: www.hermanmiller.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Herman Miller Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Herman Miller, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Herman Miller
provider_slug: herman-miller
slug: herman-miller-domain-security
source_filename: herman-miller-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hermanmiller.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 19:27:32 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: hermanmiller.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/herman-miller/refs/heads/main/security/herman-miller-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Furniture
- Design
- Office Furnishings
- Workplace
- Contract Furniture
---
