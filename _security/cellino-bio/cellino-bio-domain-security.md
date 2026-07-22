---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cellinobio.com
  spf: true
hosts:
- cert_expires: Sep  2 09:43:51 2026 GMT
  host: cellinobio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cellino Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cellino Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cellino Bio
provider_slug: cellino-bio
slug: cellino-bio-domain-security
source_filename: cellino-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cellinobio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 09:43:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cellinobio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellino-bio/refs/heads/main/security/cellino-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Regenerative Medicine
- Stem Cells
- Artificial Intelligence
- Life Sciences
- Manufacturing
---
