---
api_specs:
- filename: govconapi-com-openapi-generated.yml
  format: yaml
  label: govconapi-com API
  slug: govconapi-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govconapi-com/openapi/_ae-authored/govconapi-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: govconapi.com
  spf: true
hosts:
- cert_expires: Dec 27 00:00:49 2026 GMT
  host: govconapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Govconapi Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for govconapi-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: govconapi-com
provider_slug: govconapi-com
slug: govconapi-com-domain-security
source_filename: govconapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: govconapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 00:00:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: govconapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/govconapi-com/security/govconapi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Federal
- Procurement
- Data
- API
---
