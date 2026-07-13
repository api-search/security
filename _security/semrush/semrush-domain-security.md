---
api_specs:
- filename: semrush-openapi.yml
  format: yaml
  label: Semrush
  slug: semrush
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/openapi/semrush-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: semrush.com
  spf: true
hosts:
- cert_expires: Aug 19 18:44:32 2026 GMT
  host: developer.semrush.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 00:12:04 2026 GMT
  host: api.semrush.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Semrush Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Semrush, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Semrush
provider_slug: semrush
slug: semrush-domain-security
source_filename: semrush-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.semrush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 18:44:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.semrush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 00:12:04 2026 GMT\n  hsts: null\ndomains:\n- domain: semrush.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semrush/refs/heads/main/security/semrush-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Search Engines
---
