---
api_specs:
- filename: yapily-platform-api-openapi.yml
  format: yaml
  label: Yapily Platform API
  slug: yapily-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-platform-api-openapi.yml
- filename: yapily-institutions-api-openapi.yml
  format: yaml
  label: Yapily Institutions API
  slug: yapily-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-institutions-api-openapi.yml
- filename: yapily-consents-api-openapi.yml
  format: yaml
  label: Yapily Consents and Authorisations API
  slug: yapily-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-consents-api-openapi.yml
- filename: yapily-data-api-openapi.yml
  format: yaml
  label: Yapily Data Access API (AIS)
  slug: yapily-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-data-api-openapi.yml
- filename: yapily-payments-api-openapi.yml
  format: yaml
  label: Yapily Payments API (PIS)
  slug: yapily-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-payments-api-openapi.yml
- filename: yapily-vrp-api-openapi.yml
  format: yaml
  label: Yapily Variable Recurring Payments API
  slug: yapily-vrp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-vrp-api-openapi.yml
- filename: yapily-hosted-pages-api-openapi.yml
  format: yaml
  label: Yapily Hosted Pages API
  slug: yapily-hosted-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-hosted-pages-api-openapi.yml
- filename: yapily-data-plus-api-openapi.yml
  format: yaml
  label: Yapily Data Plus API
  slug: yapily-data-plus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-data-plus-api-openapi.yml
- filename: yapily-beneficiaries-api-openapi.yml
  format: yaml
  label: Yapily Beneficiaries API
  slug: yapily-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-beneficiaries-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: yapily.com
  spf: true
hosts:
- cert_expires: Oct  5 17:45:25 2026 GMT
  host: www.yapily.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 06:08:50 2026 GMT
  host: docs.yapily.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 17:45:25 2026 GMT
  host: api.yapily.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yapily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yapily, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Yapily
provider_slug: yapily
slug: yapily-domain-security
source_filename: yapily-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yapily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:45:25 2026 GMT\n  hsts: false\n- host: docs.yapily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 06:08:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.yapily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:45:25 2026 GMT\n  hsts: null\ndomains:\n- domain: yapily.com\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/security/yapily-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Banking
- AISP
- PISP
- Payments
- Account Information
- Variable Recurring Payments
- Financial Services
- PSD2
- FCA
- Berlin Group
- UK
- Europe
- FinTech
---
