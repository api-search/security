---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nchromabio.com
  spf: true
hosts:
- cert_expires: Sep  8 15:59:20 2026 GMT
  host: www.nchromabio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nchroma Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nchroma Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nchroma Bio
provider_slug: nchroma-bio
slug: nchroma-bio-domain-security
source_filename: nchroma-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nchromabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 15:59:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nchromabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nchroma-bio/refs/heads/main/security/nchroma-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Genetic Medicines
- Epigenetic Editing
- Therapeutics
- Life Sciences
- Drug Discovery
---
