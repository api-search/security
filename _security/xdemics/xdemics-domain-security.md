---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xdemics.com
  spf: true
hosts:
- cert_expires: Nov 25 23:55:49 2026 GMT
  host: www.xdemics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xdemics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XDemics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: XDemics
provider_slug: xdemics
slug: xdemics-domain-security
source_filename: xdemics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xdemics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xdemics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xdemics/refs/heads/main/security/xdemics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Life Sciences
- Cell Culture
- Bioprocessing
- Cell and Gene Therapy
- Laboratory Equipment
- Manufacturing
- Hardware
- Company
---
