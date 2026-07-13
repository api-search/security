---
api_specs:
- filename: checkly-openapi.json
  format: json
  label: Checkly
  slug: checkly
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/openapi/checkly-openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: checklyhq.com
  spf: true
hosts:
- cert_expires: Oct  7 23:32:51 2026 GMT
  host: www.checklyhq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 00:34:53 2026 GMT
  host: api.checklyhq.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Checkly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Checkly, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Checkly
provider_slug: checkly
slug: checkly-domain-security
source_filename: checkly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checklyhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:32:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.checklyhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 00:34:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: checklyhq.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkly/refs/heads/main/security/checkly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Testing
---
