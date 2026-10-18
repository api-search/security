---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openclimatefix.org
  spf: true
hosts:
- cert_expires: Nov 11 16:25:44 2026 GMT
  host: openclimatefix.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Climate Fix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Climate Fix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Open Climate Fix
provider_slug: open-climate-fix
slug: open-climate-fix-domain-security
source_filename: open-climate-fix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openclimatefix.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 16:25:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openclimatefix.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-climate-fix/refs/heads/main/security/open-climate-fix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Artificial Intelligence
- Forecasting
- Climate
---
