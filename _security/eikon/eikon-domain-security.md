---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eikontx.com
  spf: true
hosts:
- cert_expires: Sep  6 22:07:40 2026 GMT
  host: www.eikontx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eikon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eikon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eikon
provider_slug: eikon
slug: eikon-domain-security
source_filename: eikon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eikontx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:07:40 2026 GMT\n  hsts: false\ndomains:\n- domain: eikontx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eikon/refs/heads/main/security/eikon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Oncology
- Life Sciences
- Microscopy
- Machine Learning
---
