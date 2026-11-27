---
api_specs:
- filename: numezis-com-openapi-generated.yml
  format: yaml
  label: Numezis API
  slug: numezis-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numezis-com/openapi/_ae-authored/numezis-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: numezis.com
  spf: true
hosts:
- cert_expires: Jan  7 12:50:21 2027 GMT
  host: numezis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Numezis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numezis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Numezis
provider_slug: numezis-com
slug: numezis-com-domain-security
source_filename: numezis-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numezis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 12:50:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: numezis.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/numezis-com/security/numezis-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accounting
- AI Agents
- Swiss SMEs
- ERP Integration
- Payroll
- VAT
- Invoicing
---
