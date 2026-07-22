---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ujet.cx
  spf: true
hosts:
- cert_expires: Sep 30 03:13:17 2026 GMT
  host: ujet.cx
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ujet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UJET, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UJET
provider_slug: ujet
slug: ujet-domain-security
source_filename: ujet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ujet.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 03:13:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ujet.cx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ujet/refs/heads/main/security/ujet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Contact Center
- CCaaS
- Customer Experience
- Artificial Intelligence
- Voice
- Messaging
- Support
---
