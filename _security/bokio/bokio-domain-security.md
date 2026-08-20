---
api_specs:
- filename: bokio-authorization-api-openapi.yml
  format: yaml
  label: Bokio authorization API
  slug: bokio-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-authorization-api-openapi.yml
- filename: bokio-bank-payments-api-openapi.yml
  format: yaml
  label: Bokio bank-payments API
  slug: bokio-bank-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-bank-payments-api-openapi.yml
- filename: bokio-chart-of-accounts-api-openapi.yml
  format: yaml
  label: Bokio chart-of-accounts API
  slug: bokio-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-chart-of-accounts-api-openapi.yml
- filename: bokio-company-information-api-openapi.yml
  format: yaml
  label: Bokio company-information API
  slug: bokio-company-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-company-information-api-openapi.yml
- filename: bokio-connections-api-openapi.yml
  format: yaml
  label: Bokio connections API
  slug: bokio-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-connections-api-openapi.yml
- filename: bokio-credit-notes-api-openapi.yml
  format: yaml
  label: Bokio credit-notes API
  slug: bokio-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-credit-notes-api-openapi.yml
- filename: bokio-customers-api-openapi.yml
  format: yaml
  label: Bokio customers API
  slug: bokio-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-customers-api-openapi.yml
- filename: bokio-fiscal-years-api-openapi.yml
  format: yaml
  label: Bokio fiscal-years API
  slug: bokio-fiscal-years-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-fiscal-years-api-openapi.yml
- filename: bokio-invoices-api-openapi.yml
  format: yaml
  label: Bokio invoices API
  slug: bokio-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-invoices-api-openapi.yml
- filename: bokio-items-api-openapi.yml
  format: yaml
  label: Bokio items API
  slug: bokio-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-items-api-openapi.yml
- filename: bokio-journal-entries-api-openapi.yml
  format: yaml
  label: Bokio journal-entries API
  slug: bokio-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-journal-entries-api-openapi.yml
- filename: bokio-sie-files-api-openapi.yml
  format: yaml
  label: Bokio sie-files API
  slug: bokio-sie-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-sie-files-api-openapi.yml
- filename: bokio-supplier-invoices-api-openapi.yml
  format: yaml
  label: Bokio supplier-invoices API
  slug: bokio-supplier-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-supplier-invoices-api-openapi.yml
- filename: bokio-suppliers-api-openapi.yml
  format: yaml
  label: Bokio suppliers API
  slug: bokio-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-suppliers-api-openapi.yml
- filename: bokio-tag-groups-api-openapi.yml
  format: yaml
  label: Bokio tag-groups API
  slug: bokio-tag-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-tag-groups-api-openapi.yml
- filename: bokio-uploads-api-openapi.yml
  format: yaml
  label: Bokio uploads API
  slug: bokio-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/openapi/bokio-uploads-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "godaddy.com"
  - 0 iodef "mailto:security@bokio.se"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bokio.se
  spf: true
hosts:
- cert_expires: Mar 30 15:41:10 2027 GMT
  host: bokio.se
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.bokio.se
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bokio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bokio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bokio
provider_slug: bokio
slug: bokio-domain-security
source_filename: bokio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bokio.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 15:41:10 2027 GMT\n  hsts: false\n- host: api.bokio.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bokio.se\n  dnssec: true\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 iodef \"mailto:security@bokio.se\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bokio/refs/heads/main/security/bokio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Accounting
- Bookkeeping
- Invoicing
- Payments
- Sweden
- SMB
- Authentication
---
