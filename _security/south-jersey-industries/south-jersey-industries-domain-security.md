---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sjindustries.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.sjindustries.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.sjindustries.com
  https: false
- host: api.sjindustries.com
  https: false
kind: domain-security
layout: security
method: probed
name: South Jersey Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for South Jersey Industries, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: South Jersey Industries
provider_slug: south-jersey-industries
slug: south-jersey-industries-domain-security
source_filename: south-jersey-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sjindustries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.sjindustries.com\n  https: false\n- host: api.sjindustries.com\n  https: false\ndomains:\n- domain: sjindustries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/south-jersey-industries/refs/heads/main/security/south-jersey-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Utilities
- Natural Gas
- Energy
---
