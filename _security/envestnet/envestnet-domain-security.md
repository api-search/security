---
api_specs:
- filename: envestnet-account-aggregation-openapi-original.yml
  format: yaml
  label: Envestnet Account Aggregation API
  slug: envestnet-account-aggregation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envestnet/refs/heads/main/openapi/envestnet-account-aggregation-openapi-original.yml
- filename: envestnet-account-token-openapi-original.yml
  format: yaml
  label: Envestnet Account Token APIs
  slug: envestnet-account-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envestnet/refs/heads/main/openapi/envestnet-account-token-openapi-original.yml
- filename: envestnet-verification-openapi-original.yml
  format: yaml
  label: Envestnet Account Verification APIs
  slug: envestnet-account-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envestnet/refs/heads/main/openapi/envestnet-verification-openapi-original.yml
- filename: envestnet-credit-accelerator-openapi-original.yml
  format: yaml
  label: Envestnet Credit Accelerator API
  slug: envestnet-credit-accelerator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envestnet/refs/heads/main/openapi/envestnet-credit-accelerator-openapi-original.yml
- filename: envestnet-insights-openapi-original.yml
  format: yaml
  label: Envestnet Insights API
  slug: envestnet-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envestnet/refs/heads/main/openapi/envestnet-insights-openapi-original.yml
- filename: envestnet-personalized-views-openapi-original.yml
  format: yaml
  label: Envestnet Personalized View API
  slug: envestnet-personalized-view-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envestnet/refs/heads/main/openapi/envestnet-personalized-views-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: envestnet.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.envestnet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: developer.envestnet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Envestnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Envestnet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Envestnet
provider_slug: envestnet
slug: envestnet-domain-security
source_filename: envestnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.envestnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\n- host: developer.envestnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: envestnet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envestnet/refs/heads/main/security/envestnet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Wealth Management
- Open Banking
- Account Aggregation
---
