---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vir.bio
  spf: true
hosts:
- cert_expires: Sep 19 12:03:21 2026 GMT
  host: www.vir.bio
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vir, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vir
provider_slug: vir
slug: vir-domain-security
source_filename: vir-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vir.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:03:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: vir.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vir/refs/heads/main/security/vir-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Tech
- Biotechnology
- Immunology
- Infectious Disease
- Oncology
- Pharmaceuticals
- Clinical Research
---
