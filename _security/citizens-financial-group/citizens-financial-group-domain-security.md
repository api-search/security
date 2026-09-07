---
api_specs:
- filename: citizens-financial-group-accounts-openapi.yml
  format: yaml
  label: Citizens Accounts API
  slug: citizens-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-accounts-openapi.yml
- filename: citizens-financial-group-statements-openapi.yml
  format: yaml
  label: Citizens Statements API
  slug: citizens-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-statements-openapi.yml
- filename: citizens-financial-group-payments-openapi.yml
  format: yaml
  label: Citizens Payments API
  slug: citizens-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-payments-openapi.yml
- filename: citizens-financial-group-account-validation-openapi.yml
  format: yaml
  label: Citizens Account Validation API
  slug: citizens-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-account-validation-openapi.yml
- filename: citizens-financial-group-account-transfer-openapi.yml
  format: yaml
  label: Citizens Account Transfer API
  slug: citizens-account-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-account-transfer-openapi.yml
- filename: citizens-financial-group-information-reporting-openapi.yml
  format: yaml
  label: Citizens Information Reporting API
  slug: citizens-information-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-information-reporting-openapi.yml
- filename: citizens-financial-group-authorize-openapi.yml
  format: yaml
  label: Citizens Authorize API
  slug: citizens-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-authorize-openapi.yml
- filename: citizens-financial-group-atm-locator-openapi.yml
  format: yaml
  label: Citizens ATM Locator API
  slug: citizens-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-atm-locator-openapi.yml
- filename: citizens-financial-group-branch-locator-openapi.yml
  format: yaml
  label: Citizens Branch Locator API
  slug: citizens-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/openapi/citizens-financial-group-branch-locator-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "ssl.com"
  - 0 issue "sectigo.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: citizensbank.com
  spf: true
hosts:
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: www.citizensbank.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: developer.citizensbank.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- host: developer-citizenspay.citizensbank.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Citizens Financial Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citizens Financial Group, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Citizens Financial Group
provider_slug: citizens-financial-group
slug: citizens-financial-group-domain-security
source_filename: citizens-financial-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.citizensbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer.citizensbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer-citizenspay.citizensbank.com\n  https: false\ndomains:\n- domain: citizensbank.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/security/citizens-financial-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Buy Now Pay Later
- Financial-Services
- FDX
- Locator
- Open Banking
- Payments
---
