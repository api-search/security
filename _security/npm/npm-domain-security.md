---
api_specs:
- filename: npm-registry-api-openapi.yml
  format: yaml
  label: npm Registry API
  slug: registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-registry-api-openapi.yml
- filename: npm-public-api-openapi.yml
  format: yaml
  label: npm Public API
  slug: public
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-public-api-openapi.yml
- filename: npm-hooks-api-openapi.yml
  format: yaml
  label: npm Hooks API
  slug: hooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/openapi/npm-hooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: npmjs.com
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: npmjs.org
  spf: true
hosts:
- cert_expires: Aug 14 03:32:50 2026 GMT
  host: www.npmjs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 19:18:50 2026 GMT
  host: registry.npmjs.org
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 18 12:15:51 2026 GMT
  host: api-docs.npmjs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Npm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for npm, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: npm
provider_slug: npm
slug: npm-domain-security
source_filename: npm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:32:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: registry.npmjs.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 19:18:50 2026 GMT\n  hsts: false\n- host: api-docs.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 12:15:51 2026 GMT\n  hsts: false\ndomains:\n- domain: npmjs.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: npmjs.org\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\
  \n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/npm/refs/heads/main/security/npm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Packages
- JavaScript
- Node.js
- Package Management
- Registry
- Security
---
