---
api_specs:
- filename: iban-test-openapi-generated.yml
  format: yaml
  label: ToadTec API
  slug: iban-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iban-test/refs/heads/main/openapi/_ae-authored/iban-test-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iban-test.eu
  spf: true
hosts:
- cert_expires: Jan 13 04:41:14 2027 GMT
  host: iban-test.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Iban Test Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ToadTec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ToadTec
provider_slug: iban-test
slug: iban-test-domain-security
source_filename: iban-test-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iban-test.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 04:41:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iban-test.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iban-test/refs/heads/main/security/iban-test-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Payments
- Validation
- API
---
