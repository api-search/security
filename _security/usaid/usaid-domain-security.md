---
api_specs:
- filename: api-docs
  format: yaml
  label: ForeignAssistance.gov Data API
  slug: foreignassistancegov-data-api
  spec_type: OpenAPI
  url: https://foreignassistance.gov/api-docs
description: ''
domains:
- caa:
  - 128 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 128 issue "digicert.com"
  - 128 issue "letsencrypt.org"
  - 128 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usaid.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: foreignassistance.gov
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.usaid.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: foreignassistance.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- host: data.usaid.gov
  https: false
kind: domain-security
layout: security
method: probed
name: Usaid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for USAID, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: USAID
provider_slug: usaid
slug: usaid-domain-security
source_filename: usaid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usaid.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: foreignassistance.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: data.usaid.gov\n  https: false\ndomains:\n- domain: usaid.gov\n  dnssec: true\n  caa:\n  - 128 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 128 issue \"digicert.com\"\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: foreignassistance.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usaid/refs/heads/main/security/usaid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Foreign Assistance
- International Development
- Aid Data
- Development Finance
- Global Datasets
- Government
---
