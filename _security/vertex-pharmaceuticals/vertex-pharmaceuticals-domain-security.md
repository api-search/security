---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vrtx.com
  spf: true
hosts:
- cert_expires: Aug 31 14:46:09 2026 GMT
  host: www.vrtx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 05:03:38 2026 GMT
  host: clinicaltrials.vrtx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vertex Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vertex Pharmaceuticals, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vertex Pharmaceuticals
provider_slug: vertex-pharmaceuticals
slug: vertex-pharmaceuticals-domain-security
source_filename: vertex-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vrtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 14:46:09 2026 GMT\n  hsts: null\n- host: clinicaltrials.vrtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:03:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vrtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertex-pharmaceuticals/refs/heads/main/security/vertex-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Clinical Trials
- Drug Discovery
- Healthcare
- Life Sciences
- Pharmaceuticals
---
