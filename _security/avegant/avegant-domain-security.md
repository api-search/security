---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avegant.com
  spf: true
hosts:
- cert_expires: Aug 23 05:05:29 2026 GMT
  host: avegant.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Avegant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avegant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avegant
provider_slug: avegant
slug: avegant-domain-security
source_filename: avegant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avegant.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 23 05:05:29 2026 GMT\n  hsts: false\ndomains:\n- domain: avegant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avegant/refs/heads/main/security/avegant-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Augmented Reality
- Display Technology
- Hardware
- Wearables
- AR Glasses
- Light Engine
---
