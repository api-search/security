---
api_specs:
- filename: bankid-auth-api-openapi.yml
  format: yaml
  label: BankID Auth API
  slug: bankid-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankid/refs/heads/main/openapi/bankid-auth-api-openapi.yml
- filename: bankid-cancel-api-openapi.yml
  format: yaml
  label: BankID Cancel API
  slug: bankid-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankid/refs/heads/main/openapi/bankid-cancel-api-openapi.yml
- filename: bankid-collect-api-openapi.yml
  format: yaml
  label: BankID Collect API
  slug: bankid-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankid/refs/heads/main/openapi/bankid-collect-api-openapi.yml
- filename: bankid-other-api-openapi.yml
  format: yaml
  label: BankID Other API
  slug: bankid-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankid/refs/heads/main/openapi/bankid-other-api-openapi.yml
- filename: bankid-payment-api-openapi.yml
  format: yaml
  label: BankID Payment API
  slug: bankid-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankid/refs/heads/main/openapi/bankid-payment-api-openapi.yml
- filename: bankid-phone-api-openapi.yml
  format: yaml
  label: BankID Phone API
  slug: bankid-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankid/refs/heads/main/openapi/bankid-phone-api-openapi.yml
- filename: bankid-sign-api-openapi.yml
  format: yaml
  label: BankID Sign API
  slug: bankid-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bankid/refs/heads/main/openapi/bankid-sign-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:abuse@bankid.com"
  - 128 issue "digicert.com"
  - 128 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bankid.com
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: bankid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bankid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BankID, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BankID
provider_slug: bankid
slug: bankid-domain-security
source_filename: bankid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bankid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bankid.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:abuse@bankid.com\"\n  - 128 issue \"digicert.com\"\n  - 128 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bankid/refs/heads/main/security/bankid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Authentication
- eIDAS
- Digital Identity
- Sweden
---
