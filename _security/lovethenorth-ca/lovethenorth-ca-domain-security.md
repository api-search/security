---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lovethenorth.ca
  spf: true
hosts:
- cert_expires: Dec 26 10:29:58 2026 GMT
  host: lovethenorth.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Love the North Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Love the North, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Love the North
provider_slug: lovethenorth-ca
slug: lovethenorth-ca-domain-security
source_filename: lovethenorth-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lovethenorth.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 10:29:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lovethenorth.ca\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lovethenorth-ca/security/lovethenorth-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Media
- Community
- Podcasts
- Northern Ontario
- Local News
---
