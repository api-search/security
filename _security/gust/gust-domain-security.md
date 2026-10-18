---
api_specs:
- filename: gust-accounts-api-openapi.yml
  format: yaml
  label: Gust Accounts API
  slug: gust-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gust/refs/heads/main/openapi/gust-accounts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gust.com
  spf: true
hosts:
- cert_expires: Dec 19 12:31:22 2026 GMT
  host: gust.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gust
provider_slug: gust
slug: gust-domain-security
source_filename: gust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 12:31:22 2026 GMT\n  hsts: false\ndomains:\n- domain: gust.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gust/refs/heads/main/security/gust-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Incorporation
- Equity Management
- Fundraising
- Startup Tools
- Investor Tools
- Accelerator Management
---
