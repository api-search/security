---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 64xbio.com
  spf: true
hosts:
- cert_expires: Nov  1 19:28:13 2026 GMT
  host: 64xbio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 64X Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 64x Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 64x Bio
provider_slug: 64x-bio
slug: 64x-bio-domain-security
source_filename: 64x-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 64xbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 19:28:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 64xbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/64x-bio/refs/heads/main/security/64x-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Synthetic Biology
- Gene Therapy
- Cell And Gene Therapy
- Biomanufacturing
- Cell Line Engineering
- Life Sciences
---
