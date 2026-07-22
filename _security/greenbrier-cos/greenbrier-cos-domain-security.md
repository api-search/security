---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gbrx.com
  spf: true
hosts:
- cert_expires: Aug  3 15:18:02 2026 GMT
  host: www.gbrx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Greenbrier Cos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greenbrier Companies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Greenbrier Companies
provider_slug: greenbrier-cos
slug: greenbrier-cos-domain-security
source_filename: greenbrier-cos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gbrx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  3 15:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gbrx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenbrier-cos/refs/heads/main/security/greenbrier-cos-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Rail
- Freight
- Transportation
- Manufacturing
- Leasing
---
