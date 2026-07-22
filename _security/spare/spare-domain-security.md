---
api_specs:
- filename: spare-bahrain-authentication-openapi-original.json
  format: json
  label: Spare Bahrain Authentication API
  slug: spare-bahrain-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-bahrain-authentication-openapi-original.json
- filename: spare-bahrain-ais-openapi-original.json
  format: json
  label: Spare Bahrain Account Information API
  slug: spare-bahrain-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-bahrain-ais-openapi-original.json
- filename: spare-bahrain-pis-openapi-original.json
  format: json
  label: Spare Bahrain Payment Initiation API
  slug: spare-bahrain-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-bahrain-pis-openapi-original.json
- filename: spare-ksa-authentication-openapi-original.json
  format: json
  label: Spare KSA Authentication API
  slug: spare-ksa-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-ksa-authentication-openapi-original.json
- filename: spare-ksa-ais-openapi-original.json
  format: json
  label: Spare KSA Account Information API
  slug: spare-ksa-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-ksa-ais-openapi-original.json
- filename: spare-ksa-pis-openapi-original.json
  format: json
  label: Spare KSA Payment Initiation API
  slug: spare-ksa-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-ksa-pis-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tryspare.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: tryspare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:09:40 2026 GMT
  host: docs.tryspare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: ob.tryspare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Spare
provider_slug: spare
slug: spare-domain-security
source_filename: spare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryspare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tryspare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:09:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ob.tryspare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tryspare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/security/spare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Banking
- Open Finance
- Account Information
- Payment Initiation
- AISP
- PISP
- Consent
- Bank Data
- Transactions
- Balances
- Payments
- Fintech
- MENA
- Saudi Arabia
- Bahrain
- UAE
---
