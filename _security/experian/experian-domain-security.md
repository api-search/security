---
api_specs:
- filename: experian-address-validation-api-openapi.yml
  format: yaml
  label: Experian Address Validation API
  slug: experian-address-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-address-validation-api-openapi.yml
- filename: experian-bulk-address-api-openapi.yml
  format: yaml
  label: Experian Bulk Address API
  slug: experian-bulk-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-address-api-openapi.yml
- filename: experian-bulk-email-api-openapi.yml
  format: yaml
  label: Experian Bulk Email API
  slug: experian-bulk-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-email-api-openapi.yml
- filename: experian-bulk-phone-api-openapi.yml
  format: yaml
  label: Experian Bulk Phone API
  slug: experian-bulk-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-bulk-phone-api-openapi.yml
- filename: experian-email-validation-api-openapi.yml
  format: yaml
  label: Experian Email Validation API
  slug: experian-email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-email-validation-api-openapi.yml
- filename: experian-enrichment-api-openapi.yml
  format: yaml
  label: Experian Enrichment API
  slug: experian-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-enrichment-api-openapi.yml
- filename: experian-identity-append-usa-only-api-openapi.yml
  format: yaml
  label: Experian Identity Append (USA only) API
  slug: experian-identity-append-usa-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-identity-append-usa-only-api-openapi.yml
- filename: experian-phone-validation-api-openapi.yml
  format: yaml
  label: Experian Phone Validation API
  slug: experian-phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-phone-validation-api-openapi.yml
- filename: experian-reverse-phone-append-usa-only-api-openapi.yml
  format: yaml
  label: Experian Reverse Phone Append (USA only) API
  slug: experian-reverse-phone-append-usa-only-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/openapi/experian-reverse-phone-append-usa-only-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: experianplc.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: experianaperture.io
  spf: false
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: www.experianplc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: docs.experianaperture.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.experianaperture.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Experian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Experian, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Experian
provider_slug: experian
slug: experian-domain-security
source_filename: experian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.experianplc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n- host: docs.experianaperture.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.experianaperture.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: experianplc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: experianaperture.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/experian/refs/heads/main/security/experian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Credit Bureau
- Credit Reporting
- Identity Verification
- Fraud Prevention
- Data Quality
- Address Validation
- Email Validation
- Phone Validation
- Data Enrichment
- Financial-Services
- Risk Management
---
