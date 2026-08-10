---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brightpeaktx.com
  spf: true
hosts:
- cert_expires: Oct  2 21:33:30 2026 GMT
  host: brightpeaktx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bright Peak Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright Peak Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bright Peak Therapeutics
provider_slug: bright-peak-therapeutics
slug: bright-peak-therapeutics-domain-security
source_filename: bright-peak-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brightpeaktx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:33:30 2026 GMT\n  hsts: false\ndomains:\n- domain: brightpeaktx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-peak-therapeutics/refs/heads/main/security/bright-peak-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Therapeutics
- Immunotherapy
- Oncology
- Life Sciences
- Pharmaceuticals
- Switzerland
---
