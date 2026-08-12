---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coregen.com
  spf: true
hosts:
- cert_expires: Nov  9 22:52:29 2026 GMT
  host: www.coregen.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coregen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoRegen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CoRegen
provider_slug: coregen
slug: coregen-domain-security
source_filename: coregen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coregen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 22:52:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: coregen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coregen/refs/heads/main/security/coregen-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Life Sciences
- Oncology
- Cell Therapy
- Immunotherapy
- Gene Editing
- Pharmaceuticals
- Clinical Stage
---
