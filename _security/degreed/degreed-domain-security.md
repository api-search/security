---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: degreed.com
  spf: true
hosts:
- cert_expires: Oct  3 20:32:20 2026 GMT
  host: developer.degreed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.degreed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Degreed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Degreed, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Degreed
provider_slug: degreed
slug: degreed-domain-security
source_filename: degreed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.degreed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:32:20 2026 GMT\n  hsts: null\n- host: api.degreed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: degreed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/degreed/refs/heads/main/security/degreed-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Learning Experience Platform
- Skill Development
- Learning Pathways
- Workforce Upskilling
- eLearning
- HR Technology
---
