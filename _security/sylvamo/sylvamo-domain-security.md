---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sylvamo.com
  spf: true
hosts:
- cert_expires: Aug 26 01:53:23 2026 GMT
  host: www.sylvamo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sylvamo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sylvamo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sylvamo
provider_slug: sylvamo
slug: sylvamo-domain-security
source_filename: sylvamo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sylvamo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:53:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sylvamo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sylvamo/refs/heads/main/security/sylvamo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forest Products
- Manufacturing
- Paper
- Pulp
- Sustainability
- Uncoated Freesheet
---
