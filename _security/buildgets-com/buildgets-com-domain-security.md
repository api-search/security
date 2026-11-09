---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buildgets.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: buildgets.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buildgets Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuildGets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BuildGets
provider_slug: buildgets-com
slug: buildgets-com-domain-security
source_filename: buildgets-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildgets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: buildgets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buildgets-com/security/buildgets-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Artificial Intelligence
- Budgeting
- Spanish
- Software
---
