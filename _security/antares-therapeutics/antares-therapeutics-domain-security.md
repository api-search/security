---
description: ''
domains:
- caa: []
  caa_note: No CAA records published. The initial probe recorded a resolver timeout; re-probed against 8.8.8.8 and 1.1.1.1 on 2026-07-19, both returned an empty answer.
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: antaresrx.com
  spf: true
hosts:
- cert_expires: Sep  4 13:10:50 2026 GMT
  host: antaresrx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Antares Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antares Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Antares Therapeutics
provider_slug: antares-therapeutics
slug: antares-therapeutics-domain-security
source_filename: antares-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: antaresrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 13:10:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: antaresrx.com\n  dnssec: false\n  caa: []\n  caa_note: >-\n    No CAA records published. The initial probe recorded a resolver timeout; re-probed\n    against 8.8.8.8 and 1.1.1.1 on 2026-07-19, both returned an empty answer.\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antares-therapeutics/refs/heads/main/security/antares-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Precision Medicine
- Oncology
- Drug Discovery
- Life Sciences
- Machine-Learning
---
