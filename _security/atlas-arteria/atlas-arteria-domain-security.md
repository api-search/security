---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atlasarteria.com
  spf: true
hosts:
- cert_expires: Nov 30 05:41:58 2026 GMT
  host: atlasarteria.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atlas Arteria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atlas Arteria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atlas Arteria
provider_slug: atlas-arteria
slug: atlas-arteria-domain-security
source_filename: atlas-arteria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atlasarteria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 05:41:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: atlasarteria.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlas-arteria/refs/heads/main/security/atlas-arteria-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Toll Roads
- Transportation
- Infrastructure
- Investor Relations
- ASX Listed
- Australia
---
