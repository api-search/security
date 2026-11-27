---
api_specs:
- filename: hashdit-address-intelligence-api-openapi.yml
  format: yaml
  label: HashDit Address Intelligence API
  slug: hashdit-address-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-address-intelligence-api-openapi.yml
- filename: hashdit-domain-security-api-openapi.yml
  format: yaml
  label: HashDit Domain Security API
  slug: hashdit-domain-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-domain-security-api-openapi.yml
- filename: hashdit-signature-security-api-openapi.yml
  format: yaml
  label: HashDit Signature Security API
  slug: hashdit-signature-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-signature-security-api-openapi.yml
- filename: hashdit-simulation-api-openapi.yml
  format: yaml
  label: HashDit Simulation API
  slug: hashdit-simulation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-simulation-api-openapi.yml
- filename: hashdit-token-security-api-openapi.yml
  format: yaml
  label: HashDit Token Security API
  slug: hashdit-token-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-token-security-api-openapi.yml
- filename: hashdit-transaction-security-api-openapi.yml
  format: yaml
  label: HashDit Transaction Security API
  slug: hashdit-transaction-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hashdit/openapi/hashdit-transaction-security-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hashdit.io
  spf: true
hosts:
- cert_expires: May 12 23:59:59 2027 GMT
  host: www.hashdit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HashDit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HashDit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: HashDit
provider_slug: hashdit
slug: hashdit-domain-security
source_filename: hashdit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hashdit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hashdit.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hashdit/security/hashdit-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Crypto Security
- Scam Protection
- Token Scanner
- Web3 Tools
- Monitoring Platform
---
