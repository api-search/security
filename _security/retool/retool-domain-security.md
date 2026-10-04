---
api_specs:
- filename: retool-apps-api-openapi.yml
  format: yaml
  label: Retool Apps API
  slug: retool-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/openapi/retool-apps-api-openapi.yml
- filename: retool-folders-api-openapi.yml
  format: yaml
  label: Retool Folders API
  slug: retool-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/openapi/retool-folders-api-openapi.yml
- filename: retool-groups-api-openapi.yml
  format: yaml
  label: Retool Groups API
  slug: retool-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/openapi/retool-groups-api-openapi.yml
- filename: retool-resources-api-openapi.yml
  format: yaml
  label: Retool Resources API
  slug: retool-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/openapi/retool-resources-api-openapi.yml
- filename: retool-users-api-openapi.yml
  format: yaml
  label: Retool Users API
  slug: retool-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/openapi/retool-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: retool.com
  spf: true
hosts:
- cert_expires: Nov 30 02:53:30 2026 GMT
  host: retool.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 14:30:43 2026 GMT
  host: docs.retool.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 14:04:57 2026 GMT
  host: api.retool.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Retool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Retool, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Retool
provider_slug: retool
slug: retool-domain-security
source_filename: retool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: retool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 02:53:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.retool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 14:30:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.retool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 14:04:57 2026 GMT\n  hsts: null\ndomains:\n- domain: retool.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/security/retool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Admin Panel
- Dashboards
- Internal Tools
- Low-Code
- No-Code
---
