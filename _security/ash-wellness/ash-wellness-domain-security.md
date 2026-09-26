---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: poweredbyash.com
  spf: true
hosts:
- cert_expires: Nov 10 16:55:24 2026 GMT
  host: www.poweredbyash.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ash Wellness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ash Wellness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ash Wellness
provider_slug: ash-wellness
slug: ash-wellness-domain-security
source_filename: ash-wellness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.poweredbyash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 16:55:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: poweredbyash.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ash-wellness/refs/heads/main/security/ash-wellness-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- HealthTech
- Diagnostics
- At-Home Testing
- Healthcare
- B2B
---
