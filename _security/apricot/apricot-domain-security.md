---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apricothealth.ai
  spf: true
hosts:
- cert_expires: Sep 30 18:45:26 2026 GMT
  host: www.apricothealth.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apricot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apricot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apricot
provider_slug: apricot
slug: apricot-domain-security
source_filename: apricot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apricothealth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:45:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apricothealth.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apricot/refs/heads/main/security/apricot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Home Health
- Post-Acute Care
- Clinical Documentation
- Artificial Intelligence
- HIPAA
- OASIS
---
