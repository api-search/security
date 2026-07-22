---
api_specs:
- filename: mode-openapi-original.yml
  format: yaml
  label: Mode API
  slug: mode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mode/refs/heads/main/openapi/mode-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "cloudflare.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mode.com
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: modeanalytics.com
  spf: true
hosts:
- cert_expires: Jan  9 20:00:18 2027 GMT
  host: mode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 12 19:00:20 2027 GMT
  host: app.mode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 20:00:18 2027 GMT
  host: modeanalytics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mode, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mode
provider_slug: mode
slug: mode-domain-security
source_filename: mode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mode.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 20:00:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.mode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 19:00:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: modeanalytics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 20:00:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mode.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"cloudflare.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: modeanalytics.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\
  \n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mode/refs/heads/main/security/mode-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Enterprise
- Business Intelligence
- Analytics
- Data
- Reporting
- Dashboards
- SQL
- Data Stack
---
