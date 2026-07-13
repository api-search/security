---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Locize REST API
  slug: locize-rest-api
  spec_type: OpenAPI
  url: https://www.locize.com/docs/integration/api/
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: locize.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: locize.app
  spf: true
hosts:
- cert_expires: Sep 29 11:41:16 2026 GMT
  host: www.locize.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: api.locize.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Locize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Locize, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Locize
provider_slug: locize
slug: locize-domain-security
source_filename: locize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.locize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:41:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.locize.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: locize.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: locize.app\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locize/refs/heads/main/security/locize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Localization
- Internationalization
- i18n
- Translation Management
- Translation
- i18next
- Developer Tools
- CDN
- SaaS
---
