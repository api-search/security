---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ehousestudio.com
  spf: true
hosts:
- cert_expires: Dec 13 20:57:27 2026 GMT
  host: ehousestudio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ehousestudio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eHouse Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: eHouse Studio
provider_slug: ehousestudio
slug: ehousestudio-domain-security
source_filename: ehousestudio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ehousestudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 20:57:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ehousestudio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ehousestudio/security/ehousestudio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shopify
- Agency
- Digital Commerce
- Integration
- Development
- Marketing
- Retail POS
- Strategy
---
