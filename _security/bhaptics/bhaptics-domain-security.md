---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bhaptics.com
  spf: true
hosts:
- cert_expires: Dec 26 10:32:33 2026 GMT
  host: www.bhaptics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bhaptics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bhaptics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bhaptics
provider_slug: bhaptics
slug: bhaptics-domain-security
source_filename: bhaptics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bhaptics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 10:32:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bhaptics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bhaptics/refs/heads/main/security/bhaptics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Haptics
- Wearables
- Gaming
- VR
- DeveloperTools
---
