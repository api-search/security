---
api_specs:
- filename: gospotcheck-external-openapi.yml
  format: yaml
  label: GoSpotCheck External API
  slug: gospotcheck-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/openapi/gospotcheck-external-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gospotcheck.com
  spf: true
hosts:
- cert_expires: Aug 31 10:16:08 2026 GMT
  host: gospotcheck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gospotcheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoSpotCheck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GoSpotCheck
provider_slug: gospotcheck
slug: gospotcheck-domain-security
source_filename: gospotcheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gospotcheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:16:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gospotcheck.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gospotcheck/refs/heads/main/security/gospotcheck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail Execution
- Field Service
- Data Collection
- Surveys
- Merchandising
- CPG
- Mobile
---
