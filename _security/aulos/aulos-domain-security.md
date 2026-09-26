---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aulosbio.com
  spf: true
hosts:
- cert_expires: Nov  9 14:16:41 2026 GMT
  host: aulosbio.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aulos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aulos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aulos
provider_slug: aulos
slug: aulos-domain-security
source_filename: aulos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aulosbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 14:16:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: aulosbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aulos/refs/heads/main/security/aulos-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Oncology
- Biopharma
- Antibody Therapeutics
- IL-2 Therapeutics
- Clinical Trials
---
