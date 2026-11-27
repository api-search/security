---
api_specs:
- filename: ibanchecker-cash-extract-api-openapi.yml
  format: yaml
  label: IBAN Checker Extract API
  slug: ibanchecker-cash-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ibanchecker-cash/openapi/ibanchecker-cash-extract-api-openapi.yml
- filename: ibanchecker-cash-formats-api-openapi.yml
  format: yaml
  label: IBAN Checker Formats API
  slug: ibanchecker-cash-formats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ibanchecker-cash/openapi/ibanchecker-cash-formats-api-openapi.yml
- filename: ibanchecker-cash-swift-api-openapi.yml
  format: yaml
  label: IBAN Checker Swift API
  slug: ibanchecker-cash-swift-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ibanchecker-cash/openapi/ibanchecker-cash-swift-api-openapi.yml
- filename: ibanchecker-cash-validate-api-openapi.yml
  format: yaml
  label: IBAN Checker Validate API
  slug: ibanchecker-cash-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ibanchecker-cash/openapi/ibanchecker-cash-validate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ibanchecker.cash
  spf: true
hosts:
- cert_expires: Dec 27 22:43:44 2026 GMT
  host: ibanchecker.cash
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IBAN Checker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IBAN Checker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IBAN Checker
provider_slug: ibanchecker-cash
slug: ibanchecker-cash-domain-security
source_filename: ibanchecker-cash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ibanchecker.cash\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 22:43:44 2026 GMT\n  hsts: false\ndomains:\n- domain: ibanchecker.cash\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ibanchecker-cash/security/ibanchecker-cash-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Banking
- Validation
---
