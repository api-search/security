---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 2ndbrick.com
  spf: false
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: 2ndbrick.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 2Ndbrick Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 2nd Brick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: 2nd Brick
provider_slug: 2ndbrick-com
slug: 2ndbrick-com-domain-security
source_filename: 2ndbrick-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 2ndbrick.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 2ndbrick.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/2ndbrick-com/security/2ndbrick-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Custom
- LEGO
- Design
- E-Commerce
- Artificial Intelligence
---
