---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: begonia.pro
  spf: true
hosts:
- cert_expires: Dec 31 21:13:02 2026 GMT
  host: begonia.pro
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Begonia Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Begonia.pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Begonia.pro
provider_slug: begonia-pro
slug: begonia-pro-domain-security
source_filename: begonia-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: begonia.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 21:13:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: begonia.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/begonia-pro/security/begonia-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SEO
- Local
- Artificial Intelligence
- Small Business
- Marketing
- Company
---
