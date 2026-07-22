---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forcetherapeutics.com
  spf: true
hosts:
- cert_expires: Oct 16 05:10:18 2026 GMT
  host: www.forcetherapeutics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Force Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Force Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Force Therapeutics
provider_slug: force-therapeutics
slug: force-therapeutics-domain-security
source_filename: force-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.forcetherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 05:10:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: forcetherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/force-therapeutics/refs/heads/main/security/force-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Patient Engagement
- Remote Patient Monitoring
- PROMs
- Surgical Care
- EHR Integration
- HIPAA
---
