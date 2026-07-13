---
api_specs:
- filename: avaloq-banking-openapi.yml
  format: yaml
  label: Avaloq Banking API
  slug: avaloq-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-banking-openapi.yml
- filename: avaloq-wealth-management-openapi.yml
  format: yaml
  label: Avaloq Wealth Management API
  slug: avaloq-wealth-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-wealth-management-openapi.yml
- filename: avaloq-payments-openapi.yml
  format: yaml
  label: Avaloq Payments API
  slug: avaloq-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-payments-openapi.yml
- filename: avaloq-client-management-openapi.yml
  format: yaml
  label: Avaloq Client Management API
  slug: avaloq-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-client-management-openapi.yml
- filename: avaloq-trading-openapi.yml
  format: yaml
  label: Avaloq Trading API
  slug: avaloq-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-trading-openapi.yml
- filename: avaloq-compliance-openapi.yml
  format: yaml
  label: Avaloq Compliance & Risk API
  slug: avaloq-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/openapi/avaloq-compliance-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: avaloq.com
  spf: true
hosts:
- host: developer.avaloq.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''developer.a'
- cert_expires: Aug 11 07:56:14 2026 GMT
  host: www.avaloq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.avaloq.com
  https: false
kind: domain-security
layout: security
method: probed
name: Avaloq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avaloq, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Avaloq
provider_slug: avaloq
slug: avaloq-domain-security
source_filename: avaloq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.avaloq.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''developer.a'\n  hsts: null\n- host: www.avaloq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 07:56:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.avaloq.com\n  https: false\ndomains:\n- domain: avaloq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avaloq/refs/heads/main/security/avaloq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Digital Banking
- Financial Services
- Fintech
- Payments
- Wealth Management
---
