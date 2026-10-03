---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mybinxhealth.com
  spf: true
hosts:
- cert_expires: Nov 25 21:36:20 2026 GMT
  host: mybinxhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Binx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Binx
provider_slug: binx
slug: binx-domain-security
source_filename: binx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mybinxhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 21:36:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mybinxhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binx/refs/heads/main/security/binx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Diagnostics
- Point of Care
- STI Testing
- CLIA-waived
- Company
---
