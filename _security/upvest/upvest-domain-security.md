---
api_specs:
- filename: upvest-investment-api-openapi.yml
  format: yaml
  label: Upvest Investment API
  slug: investment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upvest/refs/heads/main/openapi/upvest-investment-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: upvest.co
  spf: true
hosts:
- cert_expires: Aug 17 05:12:10 2026 GMT
  host: upvest.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 08:19:22 2026 GMT
  host: docs.upvest.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 14:51:50 2026 GMT
  host: api.upvest.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upvest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upvest, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Upvest
provider_slug: upvest
slug: upvest-domain-security
source_filename: upvest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upvest.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 05:12:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.upvest.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 08:19:22 2026 GMT\n  hsts: false\n- host: api.upvest.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 14:51:50 2026 GMT\n  hsts: null\ndomains:\n- domain: upvest.co\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upvest/refs/heads/main/security/upvest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking Infrastructure
- Fintech
- Investments
- Securities
- Fractional Investing
- Custody
- Wealth Management
---
