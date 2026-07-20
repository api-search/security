---
api_specs:
- filename: dash0-openapi.json
  format: json
  label: Dash0 API
  slug: dash0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dash0/refs/heads/main/openapi/dash0-openapi.json
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dash0.com
  spf: true
hosts:
- cert_expires: Aug 18 10:35:42 2026 GMT
  host: www.dash0.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 02:32:40 2026 GMT
  host: api-docs.dash0.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 05:22:03 2026 GMT
  host: api.eu-west-1.aws.dash0.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dash0 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dash0, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dash0
provider_slug: dash0
slug: dash0-domain-security
source_filename: dash0-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dash0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 10:35:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.dash0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 02:32:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.eu-west-1.aws.dash0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 05:22:03 2026 GMT\n  hsts: null\ndomains:\n- domain: dash0.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dash0/refs/heads/main/security/dash0-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Observability
- OpenTelemetry
- Monitoring
- Logs
- Metrics
- Tracing
- APM
- Prometheus
- DevOps
- Company
- Apis
---
