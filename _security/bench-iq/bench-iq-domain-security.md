---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: benchiq.com
  spf: true
hosts:
- cert_expires: Oct 10 23:39:43 2026 GMT
  host: www.benchiq.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bench Iq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bench IQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bench IQ
provider_slug: bench-iq
slug: bench-iq-domain-security
source_filename: bench-iq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.benchiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:39:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: benchiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bench-iq/refs/heads/main/security/bench-iq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Legal Tech
- Artificial Intelligence
- Judicial Analytics
- Litigation
- Legal Research
---
