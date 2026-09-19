---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ferro.com
  spf: true
hosts:
- cert_expires: Nov 24 08:10:02 2026 GMT
  host: www.ferro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.ferro.com
  https: false
- host: api.ferro.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ferro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ferro Corporation, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ferro Corporation
provider_slug: ferro
slug: ferro-domain-security
source_filename: ferro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ferro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 08:10:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ferro.com\n  https: false\n- host: api.ferro.com\n  https: false\ndomains:\n- domain: ferro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ferro/refs/heads/main/security/ferro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Functional Materials
- Electronics
- Chemicals
- Specialty Chemicals
- Pigments
- Coatings
- Vibrantz Technologies
- Acquired
- Fortune 1000
---
