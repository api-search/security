---
api_specs:
- filename: timescale-analytics-api-openapi.yml
  format: yaml
  label: Timescale Analytics API
  slug: timescale-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-analytics-api-openapi.yml
- filename: timescale-auth-api-openapi.yml
  format: yaml
  label: Timescale Auth API
  slug: timescale-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-auth-api-openapi.yml
- filename: timescale-feedback-api-openapi.yml
  format: yaml
  label: Timescale Feedback API
  slug: timescale-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-feedback-api-openapi.yml
- filename: timescale-health-api-openapi.yml
  format: yaml
  label: Timescale Health API
  slug: timescale-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-health-api-openapi.yml
- filename: timescale-invites-api-openapi.yml
  format: yaml
  label: Timescale Invites API
  slug: timescale-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-invites-api-openapi.yml
- filename: timescale-pricing-api-openapi.yml
  format: yaml
  label: Timescale Pricing API
  slug: timescale-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-pricing-api-openapi.yml
- filename: timescale-projects-api-openapi.yml
  format: yaml
  label: Timescale Projects API
  slug: timescale-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-projects-api-openapi.yml
- filename: timescale-read-replica-sets-api-openapi.yml
  format: yaml
  label: Timescale Read Replica Sets API
  slug: timescale-read-replica-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-read-replica-sets-api-openapi.yml
- filename: timescale-services-api-openapi.yml
  format: yaml
  label: Timescale Services API
  slug: timescale-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-services-api-openapi.yml
- filename: timescale-spaces-api-openapi.yml
  format: yaml
  label: Timescale Spaces API
  slug: timescale-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-spaces-api-openapi.yml
- filename: timescale-vpcs-api-openapi.yml
  format: yaml
  label: Timescale VP Cs API
  slug: timescale-vpcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/openapi/timescale-vpcs-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tigerdata.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ghost.build
  spf: true
hosts:
- cert_expires: Sep 16 01:48:26 2026 GMT
  host: www.tigerdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: console.cloud.tigerdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 14:27:50 2026 GMT
  host: ghost.build
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timescale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Timescale, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Timescale
provider_slug: timescale
slug: timescale-domain-security
source_filename: timescale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tigerdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:48:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: console.cloud.tigerdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ghost.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 14:27:50 2026 GMT\n  hsts: false\ndomains:\n- domain: tigerdata.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ghost.build\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timescale/refs/heads/main/security/timescale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Database
- PostgreSQL
- Time Series
- Analytics
- Cloud Infrastructure
- Data Platform
- Vector Search
- Developer Tools
- Open Source
---
