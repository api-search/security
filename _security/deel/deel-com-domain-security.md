---
api_specs:
- filename: deel-core-api-openapi.yml
  format: yaml
  label: Deel Core API
  slug: deel-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-core-api-openapi.yml
- filename: deel-eor-api-openapi.yml
  format: yaml
  label: Deel Employer of Record (EOR) API
  slug: deel-eor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-eor-api-openapi.yml
- filename: deel-contractors-api-openapi.yml
  format: yaml
  label: Deel Contractors API
  slug: deel-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-contractors-api-openapi.yml
- filename: deel-global-payroll-api-openapi.yml
  format: yaml
  label: Deel Global Payroll API
  slug: deel-global-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-global-payroll-api-openapi.yml
- filename: deel-hris-api-openapi.yml
  format: yaml
  label: Deel HRIS API
  slug: deel-hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-hris-api-openapi.yml
- filename: deel-ats-api-openapi.yml
  format: yaml
  label: Deel ATS API
  slug: deel-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-ats-api-openapi.yml
- filename: deel-webhooks-api-openapi.yml
  format: yaml
  label: Deel Webhooks API
  slug: deel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-webhooks-api-openapi.yml
- filename: deel-platform-extensions-api-openapi.yml
  format: yaml
  label: Deel Platform Extensions API
  slug: deel-platform-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-extensions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@letsdeel.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: deel.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: letsdeel.com
  spf: true
hosts:
- cert_expires: Aug 25 11:52:29 2026 GMT
  host: www.deel.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 10:40:25 2026 GMT
  host: developer.deel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 00:38:22 2026 GMT
  host: api.letsdeel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deel Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Deel
provider_slug: deel
slug: deel-com-domain-security
source_filename: deel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 11:52:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.deel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:40:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.letsdeel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 00:38:22 2026 GMT\n  hsts: null\ndomains:\n- domain: deel.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@letsdeel.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: letsdeel.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0\
  \ issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/security/deel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- HR
- Payroll
- Global Payroll
- EOR
- Employer of Record
- Contractors
- HRIS
- ATS
- Workforce
- Compliance
- Immigration
- Background Checks
- Webhooks
- IT
---
