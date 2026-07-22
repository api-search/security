---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cubesmart.com
  spf: true
hosts:
- cert_expires: Jan 20 23:50:00 2027 GMT
  host: www.cubesmart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cubesmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CubeSmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CubeSmart
provider_slug: cubesmart
slug: cubesmart-domain-security
source_filename: cubesmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cubesmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:50:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cubesmart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubesmart/refs/heads/main/security/cubesmart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Self Storage
- Real Estate
- REIT
- Storage
- Third-Party Management
---
