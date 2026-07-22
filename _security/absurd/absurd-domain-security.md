---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: absurd.com
  spf: true
hosts:
- cert_expires: Aug 30 11:47:57 2026 GMT
  host: absurd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Absurd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Absurd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Absurd
provider_slug: absurd
slug: absurd-domain-security
source_filename: absurd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: absurd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:47:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: absurd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/absurd/refs/heads/main/security/absurd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video
- Advertising
- Marketing
- Media
- Creative
---
