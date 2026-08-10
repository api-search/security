---
api_specs:
- filename: spycloud-breach-api-openapi.yml
  format: yaml
  label: SpyCloud Breach API
  slug: spycloud-breach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-breach-api-openapi.yml
- filename: spycloud-check-api-openapi.yml
  format: yaml
  label: SpyCloud Check API
  slug: spycloud-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-check-api-openapi.yml
- filename: spycloud-compass-api-openapi.yml
  format: yaml
  label: SpyCloud Compass API
  slug: spycloud-compass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-compass-api-openapi.yml
- filename: spycloud-data-api-openapi.yml
  format: yaml
  label: SpyCloud Data API
  slug: spycloud-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-data-api-openapi.yml
- filename: spycloud-query-api-openapi.yml
  format: yaml
  label: SpyCloud Query API
  slug: spycloud-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-query-api-openapi.yml
- filename: spycloud-stats-api-openapi.yml
  format: yaml
  label: SpyCloud Stats API
  slug: spycloud-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-stats-api-openapi.yml
- filename: spycloud-watchlist-api-openapi.yml
  format: yaml
  label: SpyCloud Watchlist API
  slug: spycloud-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-watchlist-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: spycloud.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spycloud.io
  spf: true
hosts:
- cert_expires: Oct  9 10:59:36 2026 GMT
  host: spycloud.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:31:59 2026 GMT
  host: docs.spycloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: api.spycloud.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spycloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpyCloud, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SpyCloud
provider_slug: spycloud
slug: spycloud-domain-security
source_filename: spycloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spycloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 10:59:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.spycloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:31:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spycloud.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spycloud.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: spycloud.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/security/spycloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cybersecurity
- Threat Intelligence
- Identity
- Fraud Prevention
- Account Takeover
- Dark Web
- Breach Data
- Malware
- Authentication
- Security
---
