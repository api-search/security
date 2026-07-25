---
api_specs:
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Chase UK Account and Transaction Information API (AIS)
  slug: chase-uk-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase-uk/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Chase UK Payment Initiation API (PIS)
  slug: chase-uk-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase-uk/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Chase UK Confirmation of Funds API (CBPII)
  slug: chase-uk-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase-uk/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chase.co.uk
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: www.chase.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: developer.openbanking-obie-sandbox.chase.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chase Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chase UK, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chase UK
provider_slug: chase-uk
slug: chase-uk-domain-security
source_filename: chase-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chase.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.openbanking-obie-sandbox.chase.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chase.co.uk\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chase-uk/refs/heads/main/security/chase-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Fintech
---
