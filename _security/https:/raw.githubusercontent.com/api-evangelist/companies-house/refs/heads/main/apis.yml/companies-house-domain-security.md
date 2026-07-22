---
api_specs:
- filename: specs.developer.ch.gov.uk
  format: yaml
  label: Companies House Public Data API
  slug: companies-house-public-data-api
  spec_type: OpenAPI
  url: https://github.com/companieshouse/specs.developer.ch.gov.uk
description: ''
domains:
- caa:
  - www-cdn.production.govuk.service.gov.uk.
  - www-gov-uk.map.fastly.net.
  dmarc: false
  dnssec: true
  domain: www.gov.uk
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: service.gov.uk
  spf: true
hosts:
- cert_expires: Dec 28 22:06:14 2026 GMT
  host: www.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: developer.company-information.service.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: api.company-information.service.gov.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Companies House Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Companies House, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Companies House
provider_slug: https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/apis.yml
slug: companies-house-domain-security
source_filename: companies-house-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 22:06:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.company-information.service.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.company-information.service.gov.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: www.gov.uk\n  dnssec: true\n  caa:\n  - www-cdn.production.govuk.service.gov.uk.\n  - www-gov-uk.map.fastly.net.\n  spf: false\n  dmarc: false\n- domain: service.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/https://raw.githubusercontent.com/api-evangelist/companies-house/refs/heads/main/apis.yml/refs/heads/main/security/companies-house-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Companies
- UK Government
- Business Registration
- Company Search
- Officers
- Filing History
- Insolvency
- Charges
- Persons of Significant Control
- Open Data
---
