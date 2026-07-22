---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: octant.bio
  spf: true
hosts:
- cert_expires: Sep  5 05:09:11 2026 GMT
  host: www.octant.bio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Octant Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octant Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Octant Bio
provider_slug: octant-bio
slug: octant-bio-domain-security
source_filename: octant-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.octant.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:09:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: octant.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octant-bio/refs/heads/main/security/octant-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Precision Medicine
- Drug Discovery
- Therapeutics
- Synthetic Biology
- Pharmaceuticals
- Life Sciences
---
