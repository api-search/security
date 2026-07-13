---
api_specs:
- filename: lemlist-openapi.yml
  format: yaml
  label: lemlist REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/openapi/lemlist-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lemlist.com
  spf: true
hosts:
- cert_expires: Sep 19 01:21:21 2026 GMT
  host: www.lemlist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 21:49:45 2026 GMT
  host: developer.lemlist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 17:35:20 2026 GMT
  host: api.lemlist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemlist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lemlist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: lemlist
provider_slug: lemlist
slug: lemlist-domain-security
source_filename: lemlist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lemlist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 01:21:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.lemlist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:49:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lemlist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:35:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lemlist.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemlist/refs/heads/main/security/lemlist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Outreach
- Sales Engagement
- Cold Email
- Sales Automation
- LinkedIn Outreach
- Lead Generation
---
