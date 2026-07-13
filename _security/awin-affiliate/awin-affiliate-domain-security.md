---
api_specs:
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Accounts API
  slug: awin-affiliate-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Transactions API
  slug: awin-affiliate-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Reports API
  slug: awin-affiliate-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Commission Groups API
  slug: awin-affiliate-commission-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
- filename: awin-affiliate-openapi.yml
  format: yaml
  label: Awin Programmes API
  slug: awin-affiliate-programmes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/openapi/awin-affiliate-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: awin.com
  spf: true
hosts:
- cert_expires: Oct  6 11:37:45 2026 GMT
  host: www.awin.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 14:25:52 2026 GMT
  host: help.awin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 11:37:45 2026 GMT
  host: api.awin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Awin Affiliate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Awin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Awin
provider_slug: awin-affiliate
slug: awin-affiliate-domain-security
source_filename: awin-affiliate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.awin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:37:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: help.awin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 14:25:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.awin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:37:45 2026 GMT\n  hsts: null\ndomains:\n- domain: awin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awin-affiliate/refs/heads/main/security/awin-affiliate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate Marketing
- Advertising
- Publishers
- Advertisers
- Transactions
- Reporting
- Commissions
- Performance Marketing
---
