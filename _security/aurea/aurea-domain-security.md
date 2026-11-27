---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aurea.com
  spf: true
hosts:
- cert_expires: Dec 26 12:36:11 2026 GMT
  host: www.aurea.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aurea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aurea
provider_slug: aurea
slug: aurea-domain-security
source_filename: aurea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aurea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 12:36:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aurea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aurea/security/aurea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software
- Enterprise
- Artificial Intelligence
- Cloud
---
