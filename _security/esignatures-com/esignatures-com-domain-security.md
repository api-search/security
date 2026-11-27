---
api_specs:
- filename: esignatures-com-openapi-generated.yml
  format: yaml
  label: eSignatures.com API
  slug: esignatures-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esignatures-com/openapi/_ae-authored/esignatures-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: esignatures.com
  spf: true
hosts:
- cert_expires: Mar 29 23:59:59 2027 GMT
  host: esignatures.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: eSignatures.com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eSignatures.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: eSignatures.com
provider_slug: esignatures-com
slug: esignatures-com-domain-security
source_filename: esignatures-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: esignatures.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: esignatures.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/esignatures-com/security/esignatures-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Signature
- Compliance
- MobileFirst
- Bulk Sending
- Integration
- AI-native
---
