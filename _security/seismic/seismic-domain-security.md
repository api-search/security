---
api_specs:
- filename: seismic-content-openapi.yml
  format: yaml
  label: Seismic Content API
  slug: seismic-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-content-openapi.yml
- filename: seismic-livedocs-openapi.yml
  format: yaml
  label: Seismic LiveDocs API
  slug: seismic-livedocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-livedocs-openapi.yml
- filename: seismic-analytics-openapi.yml
  format: yaml
  label: Seismic Analytics API
  slug: seismic-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-analytics-openapi.yml
- filename: seismic-user-management-openapi.yml
  format: yaml
  label: Seismic User Management API
  slug: seismic-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/openapi/seismic-user-management-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:security@seismic.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: seismic.com
  spf: true
hosts:
- cert_expires: Oct  2 21:07:53 2026 GMT
  host: developer.seismic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:45:09 2026 GMT
  host: seismic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 23:59:59 2026 GMT
  host: api.seismic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seismic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seismic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Seismic
provider_slug: seismic
slug: seismic-domain-security
source_filename: seismic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.seismic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:07:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: seismic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:45:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.seismic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: seismic.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:security@seismic.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/security/seismic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
