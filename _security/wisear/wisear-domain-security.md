---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wisear.io
  spf: true
hosts:
- cert_expires: Sep 16 00:55:16 2026 GMT
  host: wisear.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wisear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wisear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wisear
provider_slug: wisear
slug: wisear-domain-security
source_filename: wisear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wisear.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:55:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wisear.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisear/refs/heads/main/security/wisear-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Neural Interface
- Brain-Computer Interface
- Wearables
- Hands-Free Controls
- AR/VR
- Artificial Intelligence
- Accessibility
---
