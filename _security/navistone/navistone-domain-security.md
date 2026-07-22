---
api_specs:
- filename: navistone-openapi-original.json
  format: json
  label: NaviStone Platform API
  slug: navistone-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/openapi/navistone-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: navistone.com
  spf: true
hosts:
- cert_expires: Sep 20 19:12:43 2026 GMT
  host: www.navistone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Navistone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NaviStone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NaviStone
provider_slug: navistone
slug: navistone-domain-security
source_filename: navistone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.navistone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:12:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: navistone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navistone/refs/heads/main/security/navistone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Direct Mail
- Advertising
- Customer Acquisition
- Audience Targeting
- MarTech
- AdTech
- Postcards
- Retargeting
---
