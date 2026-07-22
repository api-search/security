---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: phasevtrials.com
  spf: true
hosts:
- cert_expires: Sep 26 10:21:52 2026 GMT
  host: www.phasevtrials.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phasev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PhaseV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: PhaseV
provider_slug: phasev
slug: phasev-domain-security
source_filename: phasev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.phasevtrials.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 10:21:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: phasevtrials.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phasev/refs/heads/main/security/phasev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Ai
- Clinical Trials
- Biopharma
- Machine Learning
- Life Sciences
- Healthcare
- Drug Development
---
