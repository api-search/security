---
api_specs:
- filename: bike4mind-com-openapi.json
  format: json
  label: Bike4Mind API
  slug: bike4mind-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bike4mind-com/openapi/bike4mind-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bike4mind.com
  spf: true
hosts:
- cert_expires: Apr 20 23:59:59 2027 GMT
  host: bike4mind.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bike4Mind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bike4Mind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bike4Mind
provider_slug: bike4mind-com
slug: bike4mind-com-domain-security
source_filename: bike4mind-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bike4mind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bike4mind.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bike4mind-com/security/bike4mind-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Open Source
- Platform
- Workbench
---
