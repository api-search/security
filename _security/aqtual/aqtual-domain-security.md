---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aqtual.com
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: aqtual.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aqtual Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aqtual, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aqtual
provider_slug: aqtual
slug: aqtual-domain-security
source_filename: aqtual-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aqtual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aqtual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aqtual/refs/heads/main/security/aqtual-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Precision Medicine
- Diagnostics
- Liquid Biopsy
- Cell-Free DNA
- Epigenetics
- Genomics
- Biotechnology
- Oncology
- Rheumatology
- Healthcare
- United States
---
