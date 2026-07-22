---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crowncork.com
  spf: true
hosts:
- cert_expires: Sep 14 12:29:51 2026 GMT
  host: www.crowncork.com
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crown Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crown Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crown Holdings
provider_slug: crown
slug: crown-domain-security
source_filename: crown-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crowncork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:29:51 2026 GMT\n  hsts: true\n  hsts_max_age: 1000\ndomains:\n- domain: crowncork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crown/refs/heads/main/security/crown-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aerosol Cans
- Beverage Cans
- Closures
- Consumer Goods
- Food Cans
- Manufacturing
- Metal Packaging
- Packaging
- Protective Packaging
- Specialty Packaging
- Sustainability
- Transit Packaging
- Fortune 500
---
