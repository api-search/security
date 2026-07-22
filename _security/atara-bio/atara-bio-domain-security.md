---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atarabio.com
  spf: true
hosts:
- cert_expires: Oct 12 11:03:17 2026 GMT
  host: www.atarabio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atara Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atara Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Atara Bio
provider_slug: atara-bio
slug: atara-bio-domain-security
source_filename: atara-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atarabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 11:03:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atarabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atara-bio/refs/heads/main/security/atara-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Biotechnology
- Immunotherapy
- Cell Therapy
- Pharmaceuticals
- Life Sciences
---
