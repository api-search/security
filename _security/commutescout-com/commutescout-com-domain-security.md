---
api_specs:
- filename: commutescout-com-tools-api-openapi.yml
  format: yaml
  label: CommuteScout Tools API
  slug: commutescout-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commutescout-com/openapi/commutescout-com-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commutescout.com
  spf: true
hosts:
- cert_expires: Dec 23 14:53:03 2026 GMT
  host: commutescout.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CommuteScout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CommuteScout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CommuteScout
provider_slug: commutescout-com
slug: commutescout-com-domain-security
source_filename: commutescout-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commutescout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 14:53:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: commutescout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/commutescout-com/security/commutescout-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Traffic
- Road Conditions
- Transportation
- Navigation
- Route Planning
- Maps
- MCP
- Open Source
---
