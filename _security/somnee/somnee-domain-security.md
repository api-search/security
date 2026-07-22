---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: somneesleep.com
  spf: true
hosts:
- cert_expires: Sep 14 18:16:03 2026 GMT
  host: somneesleep.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Somnee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Somnee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Somnee
provider_slug: somnee
slug: somnee-domain-security
source_filename: somnee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: somneesleep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:16:03 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: somneesleep.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/somnee/refs/heads/main/security/somnee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sleep
- Sleep Technology
- Neurotechnology
- Neurostimulation
- Wearables
- Digital Health
- EEG
- Consumer Electronics
---
