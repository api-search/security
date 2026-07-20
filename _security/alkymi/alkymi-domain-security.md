---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alkymi.io
  spf: true
hosts:
- cert_expires: Aug 26 05:38:35 2026 GMT
  host: www.alkymi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alkymi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alkymi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alkymi
provider_slug: alkymi
slug: alkymi-domain-security
source_filename: alkymi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alkymi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 05:38:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alkymi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alkymi/refs/heads/main/security/alkymi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Private Markets
- Document Processing
- Data Extraction
- Artificial Intelligence
- Alternative Investments
- Webhooks
---
