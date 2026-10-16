---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: smhi.se
  spf: true
hosts:
- cert_expires: Nov 28 04:01:35 2026 GMT
  host: www.smhi.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smhi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMHI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SMHI
provider_slug: smhi
slug: smhi-domain-security
source_filename: smhi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smhi.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 04:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smhi.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smhi/refs/heads/main/security/smhi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Weather
- Climate
- Data
- Research
- Sweden
---
