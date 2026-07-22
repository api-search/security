---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: culdesac.com
  spf: true
hosts:
- cert_expires: Aug 20 04:16:35 2026 GMT
  host: culdesac.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Culdesac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Culdesac, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Culdesac
provider_slug: culdesac
slug: culdesac-domain-security
source_filename: culdesac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: culdesac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:16:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: culdesac.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culdesac/refs/heads/main/security/culdesac-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Real Estate Development
- Housing
- Urban Planning
- Car-Free
- Mobility
- Property Management
---
