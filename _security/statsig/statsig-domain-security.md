---
api_specs:
- filename: statsig-http-api-openapi.yml
  format: yaml
  label: Statsig HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-http-api-openapi.yml
- filename: statsig-console-api-openapi.yml
  format: yaml
  label: Statsig Console API
  slug: console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-console-api-openapi.yml
- filename: statsig-client-sdk-api-openapi.yml
  format: yaml
  label: Statsig Client SDK API
  slug: client-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-client-sdk-api-openapi.yml
- filename: statsig-server-sdk-api-openapi.yml
  format: yaml
  label: Statsig Server SDK API
  slug: server-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-server-sdk-api-openapi.yml
- filename: statsig-events-api-openapi.yml
  format: yaml
  label: Statsig Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/openapi/statsig-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: statsig.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: statsigapi.net
  spf: false
hosts:
- cert_expires: Sep 15 16:23:32 2026 GMT
  host: docs.statsig.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 17:15:26 2026 GMT
  host: api.statsig.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 12:30:25 2026 GMT
  host: statsigapi.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Statsig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for statsig, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: statsig
provider_slug: statsig
slug: statsig-domain-security
source_filename: statsig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.statsig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:23:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.statsig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 17:15:26 2026 GMT\n  hsts: null\n- host: statsigapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 12:30:25 2026 GMT\n  hsts: null\ndomains:\n- domain: statsig.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: statsigapi.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/statsig/refs/heads/main/security/statsig-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
