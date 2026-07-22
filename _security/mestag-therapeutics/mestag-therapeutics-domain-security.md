---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mestagtx.com
  spf: true
hosts:
- cert_expires: Oct  2 07:34:02 2026 GMT
  host: mestagtx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mestag Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mestag Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mestag Therapeutics
provider_slug: mestag-therapeutics
slug: mestag-therapeutics-domain-security
source_filename: mestag-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mestagtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:34:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mestagtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mestag-therapeutics/refs/heads/main/security/mestag-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Immunology
- Immunotherapy
- Oncology
- Drug Discovery
- Inflammatory Disease
- Antibodies
- Cambridge UK
---
