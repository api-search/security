---
api_specs:
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Auth & Link API
  slug: okra-ng-auth-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Accounts & Balance API
  slug: okra-ng-accounts-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Transactions API
  slug: okra-ng-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Identity & Income API
  slug: okra-ng-identity-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Payments API
  slug: okra-ng-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
- filename: okra-ng-openapi.yml
  format: yaml
  label: Okra Webhooks API
  slug: okra-ng-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/openapi/okra-ng-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: okra.ng
  spf: true
hosts:
- host: okra.ng
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''okra.ng''. ('
- host: docs.okra.ng
  https: false
- host: api.okra.ng
  https: false
kind: domain-security
layout: security
method: probed
name: Okra Ng Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Okra, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Okra
provider_slug: okra-ng
slug: okra-ng-domain-security
source_filename: okra-ng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: okra.ng\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''okra.ng''. ('\n  hsts: null\n- host: docs.okra.ng\n  https: false\n- host: api.okra.ng\n  https: false\ndomains:\n- domain: okra.ng\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okra-ng/refs/heads/main/security/okra-ng-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Open Banking
- Open Finance
- Fintech
- Africa
- Nigeria
- Financial Data
---
