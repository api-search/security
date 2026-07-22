---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: altatech.io
  spf: true
hosts:
- cert_expires: Aug 18 17:44:02 2026 GMT
  host: altatech.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alta Resource Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alta Resource Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alta Resource Technologies
provider_slug: alta-resource-technologies
slug: alta-resource-technologies-domain-security
source_filename: alta-resource-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: altatech.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 17:44:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: altatech.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alta-resource-technologies/refs/heads/main/security/alta-resource-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Critical Minerals
- Rare Earth Elements
- Biotechnology
- Mining
- Materials Science
- Clean Technology
- Recycling
- Supply Chain
---
