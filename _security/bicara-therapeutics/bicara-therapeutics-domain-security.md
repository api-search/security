---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bicara.com
  spf: true
hosts:
- cert_expires: Oct 31 12:12:04 2026 GMT
  host: www.bicara.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bicara Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bicara Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bicara Therapeutics
provider_slug: bicara-therapeutics
slug: bicara-therapeutics-domain-security
source_filename: bicara-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bicara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 12:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bicara.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bicara-therapeutics/refs/heads/main/security/bicara-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Gene Editing
- Therapeutics
- Rare Disease
- Oncology
---
