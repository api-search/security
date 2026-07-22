---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: optimal.lat
  spf: true
hosts:
- cert_expires: Oct 10 00:50:02 2026 GMT
  host: optimal.lat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optimal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optimal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Optimal
provider_slug: optimal
slug: optimal-domain-security
source_filename: optimal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: optimal.lat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:50:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: optimal.lat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimal/refs/heads/main/security/optimal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Preventive Health
- Longevity
- Biomarkers
- Diagnostics
- Wellness
- Latin America
- Artificial Intelligence
---
