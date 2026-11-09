---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deepidv.com
  spf: true
hosts:
- cert_expires: Dec 30 19:56:56 2026 GMT
  host: www.deepidv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deepidv Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deep Identity Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Deep Identity Inc.
provider_slug: deepidv-com
slug: deepidv-com-domain-security
source_filename: deepidv-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deepidv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:56:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deepidv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/deepidv-com/security/deepidv-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Identity Verification
- Fraud Prevention
- Biometrics
- Deepfake Detection
---
