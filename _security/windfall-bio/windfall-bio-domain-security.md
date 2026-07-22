---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: windfall.bio
  spf: true
hosts:
- cert_expires: Sep  6 09:26:02 2026 GMT
  host: www.windfall.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Windfall Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Windfall Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Windfall Bio
provider_slug: windfall-bio
slug: windfall-bio-domain-security
source_filename: windfall-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.windfall.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:26:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: windfall.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windfall-bio/refs/heads/main/security/windfall-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Deep Tech
- Climate Tech
- Methane
- Biotech
- Agriculture
- Carbon Credits
---
