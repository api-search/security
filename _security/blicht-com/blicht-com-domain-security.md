---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blicht.com
  spf: true
hosts:
- cert_expires: Dec 14 23:46:46 2026 GMT
  host: blicht.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blicht Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BLICHT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BLICHT
provider_slug: blicht-com
slug: blicht-com-domain-security
source_filename: blicht-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blicht.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:46:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: blicht.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blicht-com/security/blicht-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- KI
- Alltag
- Technologie
- Wirtschaft
---
