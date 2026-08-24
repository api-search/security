---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lbpharma.us
  spf: true
hosts:
- cert_expires: Nov 10 23:04:44 2026 GMT
  host: lbpharma.us
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lb Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LB Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LB Pharmaceuticals
provider_slug: lb-pharmaceuticals
slug: lb-pharmaceuticals-domain-security
source_filename: lb-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lbpharma.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:04:44 2026 GMT\n  hsts: false\ndomains:\n- domain: lbpharma.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lb-pharmaceuticals/refs/heads/main/security/lb-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Life Sciences
- Health
- Clinical Trials
- Neuroscience
- Drug Development
---
