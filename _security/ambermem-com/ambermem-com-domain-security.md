---
api_specs:
- filename: ambermem-com-openapi-generated.yml
  format: yaml
  label: Amber API
  slug: ambermem-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ambermem-com/openapi/_ae-authored/ambermem-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ambermem.com
  spf: true
hosts:
- cert_expires: Jan 27 04:25:11 2027 GMT
  host: ambermem.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amber
provider_slug: ambermem-com
slug: ambermem-com-domain-security
source_filename: ambermem-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ambermem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 04:25:11 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ambermem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ambermem-com/security/ambermem-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Memory
- Subscription
- MCP
- Personal Data
---
