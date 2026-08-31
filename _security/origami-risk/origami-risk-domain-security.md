---
api_specs:
- filename: origami-risk-authentication-api-openapi.yml
  format: yaml
  label: Origami Risk Authentication API
  slug: origami-risk-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-authentication-api-openapi.yml
- filename: origami-risk-hastokenexpired-api-openapi.yml
  format: yaml
  label: Origami Risk Has Token Expired API
  slug: origami-risk-hastokenexpired-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-hastokenexpired-api-openapi.yml
- filename: origami-risk-new-endpoint-1-api-openapi.yml
  format: yaml
  label: Origami Risk New Endpoint 1 API
  slug: origami-risk-new-endpoint-1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-new-endpoint-1-api-openapi.yml
- filename: origami-risk-new-endpoint-api-openapi.yml
  format: yaml
  label: Origami Risk New Endpoint API
  slug: origami-risk-new-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-new-endpoint-api-openapi.yml
- filename: origami-risk-requests-api-openapi.yml
  format: yaml
  label: Origami Risk Requests API
  slug: origami-risk-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-requests-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: origamirisk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dais.com
  spf: true
hosts:
- cert_expires: Sep  3 12:43:46 2026 GMT
  host: www.origamirisk.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 20:12:22 2026 GMT
  host: developers.origamirisk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: origamirater-standard.dev.dais.com
  https: false
kind: domain-security
layout: security
method: probed
name: Origami Risk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Origami Risk, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Origami Risk
provider_slug: origami-risk
slug: origami-risk-domain-security
source_filename: origami-risk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.origamirisk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 12:43:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developers.origamirisk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:12:22 2026 GMT\n  hsts: null\n- host: origamirater-standard.dev.dais.com\n  https: false\ndomains:\n- domain: origamirisk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dais.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/security/origami-risk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- United States
- Property and Casualty
- Policy Administration
- Claims
- Underwriting
- Core Systems
- Risk Management
- Workers Compensation
- Insurtech
- Billing
---
