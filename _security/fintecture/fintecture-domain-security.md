---
api_specs:
- filename: fintecture-pis-api-openapi.yml
  format: yaml
  label: Fintecture Payment Initiation Services API
  slug: fintecture-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-pis-api-openapi.yml
- filename: fintecture-ais-api-openapi.yml
  format: yaml
  label: Fintecture Account Information Services API
  slug: fintecture-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-ais-api-openapi.yml
- filename: fintecture-customers-api-openapi.yml
  format: yaml
  label: Fintecture Customers API
  slug: fintecture-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-customers-api-openapi.yml
- filename: fintecture-emandates-api-openapi.yml
  format: yaml
  label: Fintecture E-Mandates API
  slug: fintecture-emandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-emandates-api-openapi.yml
- filename: fintecture-oauth-api-openapi.yml
  format: yaml
  label: Fintecture OAuth and Tokens API
  slug: fintecture-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-oauth-api-openapi.yml
- filename: fintecture-resources-api-openapi.yml
  format: yaml
  label: Fintecture Resources API
  slug: fintecture-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-resources-api-openapi.yml
- filename: fintecture-oac-api-openapi.yml
  format: yaml
  label: Fintecture Organisation Access Credentials API
  slug: fintecture-oac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-oac-api-openapi.yml
- filename: fintecture-transactions-api-openapi.yml
  format: yaml
  label: Fintecture Transactions and Settlements API
  slug: fintecture-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/openapi/fintecture-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "actalis.it"
  - 0 issue "multicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fintecture.com
  spf: true
hosts:
- cert_expires: Sep 17 17:52:47 2026 GMT
  host: fintecture.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 05:57:50 2026 GMT
  host: doc.fintecture.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 19:42:41 2026 GMT
  host: api.fintecture.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fintecture Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fintecture, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fintecture
provider_slug: fintecture
slug: fintecture-domain-security
source_filename: fintecture-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fintecture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:52:47 2026 GMT\n  hsts: null\n- host: doc.fintecture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 05:57:50 2026 GMT\n  hsts: null\n- host: api.fintecture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 19:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: fintecture.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"actalis.it\"\n  - 0 issue \"multicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fintecture/refs/heads/main/security/fintecture-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Banking
- Payments
- PSD2
- France
- Account Information
- Payment Initiation
- Instant Payments
- SEPA
- Smart Transfer
- Request To Pay
- Buy Now Pay Later
- E-Mandates
- Account-to-Account
- KYC
---
