---
api_specs:
- filename: consentstack-io-openapi-generated.yml
  format: yaml
  label: ConsentStack API
  slug: consentstack-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/consentstack-io/openapi/_ae-authored/consentstack-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: consentstack.io
  spf: true
hosts:
- cert_expires: Jan 28 22:45:10 2027 GMT
  host: consentstack.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Consentstack Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConsentStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ConsentStack
provider_slug: consentstack-io
slug: consentstack-io-domain-security
source_filename: consentstack-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: consentstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 22:45:10 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: consentstack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/consentstack-io/security/consentstack-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consent Management
- Privacy
- GDPR
- CCPA
- Cookie
---
