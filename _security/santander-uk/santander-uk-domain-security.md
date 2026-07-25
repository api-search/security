---
api_specs:
- filename: obie-opendata-swagger.json
  format: json
  label: Santander UK Open Data API
  slug: santander-uk-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santander-uk/refs/heads/main/openapi/obie-opendata-swagger.json
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Santander UK Account & Transaction Information API
  slug: santander-uk-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santander-uk/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Santander UK Payment Initiation API
  slug: santander-uk-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santander-uk/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Santander UK Confirmation of Funds API
  slug: santander-uk-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santander-uk/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: santander.co.uk
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.santander.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 22:05:49 2026 GMT
  host: api-portal.omni.slz.santander.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 03:35:27 2026 GMT
  host: developer.santander.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Santander Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Santander UK, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Santander UK
provider_slug: santander-uk
slug: santander-uk-domain-security
source_filename: santander-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.santander.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\n- host: api-portal.omni.slz.santander.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 22:05:49 2026 GMT\n  hsts: null\n- host: developer.santander.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 03:35:27 2026 GMT\n  hsts: null\ndomains:\n- domain: santander.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/santander-uk/refs/heads/main/security/santander-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
- FAPI
---
