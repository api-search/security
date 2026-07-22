---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: super.gs
  spf: true
hosts:
- cert_expires: Oct 11 13:29:03 2026 GMT
  host: super.gs
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Super Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Super, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Super
provider_slug: super
slug: super-domain-security
source_filename: super-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: super.gs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:29:03 2026 GMT\n  hsts: false\ndomains:\n- domain: super.gs\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super/refs/heads/main/security/super-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Entertainment
- Consumer
- Mobile
- Gaming
- Rewards
---
