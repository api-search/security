---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lugg.com
  spf: true
hosts:
- cert_expires: Sep 13 07:13:07 2026 GMT
  host: lugg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 05:26:01 2026 GMT
  host: docs.lugg.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 08:43:25 2026 GMT
  host: api.lugg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lugg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lugg, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lugg
provider_slug: lugg
slug: lugg-domain-security
source_filename: lugg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lugg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 07:13:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.lugg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 05:26:01 2026 GMT\n  hsts: false\n- host: api.lugg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:43:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lugg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lugg/refs/heads/main/security/lugg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Delivery
- Moving
- Last Mile
- Transportation
- On-Demand
- Webhooks
---
