---
api_specs:
- filename: beecargo-net-agent-api-openapi.yml
  format: yaml
  label: Beecargo Agent API
  slug: beecargo-net-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-agent-api-openapi.yml
- filename: beecargo-net-connect-api-openapi.yml
  format: yaml
  label: Beecargo Connect API
  slug: beecargo-net-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-connect-api-openapi.yml
- filename: beecargo-net-downloads-api-openapi.yml
  format: yaml
  label: Beecargo Downloads API
  slug: beecargo-net-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-downloads-api-openapi.yml
- filename: beecargo-net-files-api-openapi.yml
  format: yaml
  label: Beecargo Files API
  slug: beecargo-net-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-files-api-openapi.yml
- filename: beecargo-net-folders-api-openapi.yml
  format: yaml
  label: Beecargo Folders API
  slug: beecargo-net-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-folders-api-openapi.yml
- filename: beecargo-net-system-api-openapi.yml
  format: yaml
  label: Beecargo System API
  slug: beecargo-net-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beecargo-net/openapi/beecargo-net-system-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beecargo.net
  spf: false
hosts:
- cert_expires: Jan  3 17:14:23 2027 GMT
  host: beecargo.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beecargo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beecargo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Beecargo
provider_slug: beecargo-net
slug: beecargo-net-domain-security
source_filename: beecargo-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beecargo.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 17:14:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: beecargo.net\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/beecargo-net/security/beecargo-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- File Hosting
- Share Links
- Developers
- Agents
---
