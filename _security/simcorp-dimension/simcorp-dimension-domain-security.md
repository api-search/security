---
api_specs:
- filename: openapi.json
  format: json
  label: SimCorp Dimension Data API
  slug: simcorp-dimension-data-api
  spec_type: OpenAPI
  url: https://api.simcorp.com/dimension/v1/openapi.json
- filename: openapi.json
  format: json
  label: SimCorp Dimension Integration API
  slug: simcorp-dimension-integration-api
  spec_type: OpenAPI
  url: https://api.simcorp.com/dimension/integration/v1/openapi.json
- filename: openapi.json
  format: json
  label: SimCorp Dimension Analytics API
  slug: simcorp-dimension-analytics-api
  spec_type: OpenAPI
  url: https://api.simcorp.com/dimension/analytics/v1/openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:ssladmins@simcorp.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: simcorp.com
  spf: true
hosts:
- cert_expires: Sep 28 13:00:05 2026 GMT
  host: www.simcorp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.simcorp.com
  https: false
kind: domain-security
layout: security
method: probed
name: Simcorp Dimension Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimCorp Dimension, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SimCorp Dimension
provider_slug: simcorp-dimension
slug: simcorp-dimension-domain-security
source_filename: simcorp-dimension-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:00:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.simcorp.com\n  https: false\ndomains:\n- domain: simcorp.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:ssladmins@simcorp.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simcorp-dimension/refs/heads/main/security/simcorp-dimension-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accounting
- Asset Management
- Compliance
- Data Distribution
- Enterprise Software
- Financial Data
- Financial Technology
- Investment Management
- Portfolio Management
- Risk Management
- SimCorp One
- Streaming
- Trading
---
