---
api_specs:
- filename: chrome-stats-com-openapi.yml
  format: yaml
  label: Chrome-Stats API
  slug: chrome-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chrome-stats-com/openapi/chrome-stats-com-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: chrome-stats.com
  spf: true
hosts:
- cert_expires: Dec 16 07:34:59 2026 GMT
  host: chrome-stats.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chrome-Stats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chrome-Stats, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Chrome-Stats
provider_slug: chrome-stats-com
slug: chrome-stats-com-domain-security
source_filename: chrome-stats-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chrome-stats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 07:34:59 2026 GMT\n  hsts: null\ndomains:\n- domain: chrome-stats.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/chrome-stats-com/security/chrome-stats-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Analytics
- Extensions
- Mobile App
- Data
---
