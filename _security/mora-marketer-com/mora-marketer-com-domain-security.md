---
api_specs:
- filename: mora-marketer-com-discover-api-openapi.yml
  format: yaml
  label: Mora Discover API
  slug: mora-marketer-com-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mora-marketer-com/openapi/mora-marketer-com-discover-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mora-marketer.com
  spf: true
hosts:
- cert_expires: Feb 10 22:27:50 2027 GMT
  host: www.mora-marketer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mora
provider_slug: mora-marketer-com
slug: mora-marketer-com-domain-security
source_filename: mora-marketer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mora-marketer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 22:27:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mora-marketer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mora-marketer-com/security/mora-marketer-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Software-as-a-Service
- Social Media
- Advertising
- Content Generation
- Company
---
