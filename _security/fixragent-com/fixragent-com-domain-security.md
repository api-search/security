---
api_specs:
- filename: fixragent-com-triage-api-openapi.yml
  format: yaml
  label: fixRAgent Triage API
  slug: fixragent-com-triage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixragent-com/openapi/fixragent-com-triage-api-openapi.yml
- filename: fixragent-com-usage-api-openapi.yml
  format: yaml
  label: fixRAgent Usage API
  slug: fixragent-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixragent-com/openapi/fixragent-com-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fixragent.com
  spf: true
hosts:
- cert_expires: Jan 14 10:14:14 2027 GMT
  host: fixragent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: fixRAgent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fixRAgent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: fixRAgent
provider_slug: fixragent-com
slug: fixragent-com-domain-security
source_filename: fixragent-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixragent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 10:14:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fixragent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fixragent-com/security/fixragent-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Property Management
- Photo Triage
- Maintenance
- Real Estate
---
