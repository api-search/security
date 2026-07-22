---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abinitio-bio.com
  spf: true
hosts:
- cert_expires: Sep  5 03:45:18 2026 GMT
  host: www.abinitio-bio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abinitio Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abinitio Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Abinitio Bio
provider_slug: abinitio-bio
slug: abinitio-bio-domain-security
source_filename: abinitio-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abinitio-bio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:45:18 2026 GMT\n  hsts: false\ndomains:\n- domain: abinitio-bio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abinitio-bio/refs/heads/main/security/abinitio-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Artificial Intelligence
- Drug Manufacturing
- Machine Learning
- Pharmaceuticals
- Foundation Models
---
