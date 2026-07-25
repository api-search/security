---
api_specs:
- filename: perforce-activity-api-openapi.yml
  format: yaml
  label: Perforce Activity API
  slug: perforce-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-activity-api-openapi.yml
- filename: perforce-changes-api-openapi.yml
  format: yaml
  label: Perforce Changes API
  slug: perforce-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-changes-api-openapi.yml
- filename: perforce-comments-api-openapi.yml
  format: yaml
  label: Perforce Comments API
  slug: perforce-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-comments-api-openapi.yml
- filename: perforce-projects-api-openapi.yml
  format: yaml
  label: Perforce Projects API
  slug: perforce-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-projects-api-openapi.yml
- filename: perforce-reviews-api-openapi.yml
  format: yaml
  label: Perforce Reviews API
  slug: perforce-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-reviews-api-openapi.yml
- filename: perforce-version-api-openapi.yml
  format: yaml
  label: Perforce Version API
  slug: perforce-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-version-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: perforce.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.perforce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.perforce.com
  https: false
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: help.perforce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perforce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perforce, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Perforce
provider_slug: perforce
slug: perforce-domain-security
source_filename: perforce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.perforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.perforce.com\n  https: false\n- host: help.perforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: perforce.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/security/perforce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
