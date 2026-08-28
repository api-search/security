---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: peeltx.com
  spf: true
hosts:
- cert_expires: Oct 26 01:57:31 2026 GMT
  host: peeltx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peel Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peel Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Peel Therapeutics
provider_slug: peel-therapeutics
slug: peel-therapeutics-domain-security
source_filename: peel-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peeltx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 01:57:31 2026 GMT\n  hsts: false\ndomains:\n- domain: peeltx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peel-therapeutics/refs/heads/main/security/peel-therapeutics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Healthcare
- Oncology
- Drug Discovery
- Clinical Trials
- Research
---
