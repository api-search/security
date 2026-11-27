---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oleadesk.com
  spf: true
hosts:
- cert_expires: Dec 26 02:40:20 2026 GMT
  host: oleadesk.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OleaDesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OleaDesk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OleaDesk
provider_slug: oleadesk-com
slug: oleadesk-com-domain-security
source_filename: oleadesk-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oleadesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 02:40:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oleadesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/oleadesk-com/security/oleadesk-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Export
- Artificial Intelligence
- Email Automation
- B2B
- FoodIndustry
---
