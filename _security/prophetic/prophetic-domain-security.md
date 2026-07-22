---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prophetic.com
  spf: true
hosts:
- cert_expires: Sep 27 13:57:55 2026 GMT
  host: www.prophetic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prophetic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prophetic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prophetic
provider_slug: prophetic
slug: prophetic-domain-security
source_filename: prophetic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prophetic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 13:57:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: prophetic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prophetic/refs/heads/main/security/prophetic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Neurotechnology
- Wearables
- Consumer Hardware
- Lucid Dreaming
- Sleep Technology
- Brain-Computer Interface
- Artificial Intelligence
- Health and Wellness
---
