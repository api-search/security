---
api_specs:
- filename: refinitiv-data-platform-openapi.yml
  format: yaml
  label: Refinitiv Data Platform (RDP) API
  slug: refinitiv-data-platform-rdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/openapi/refinitiv-data-platform-openapi.yml
- filename: refinitiv-real-time-websocket-asyncapi.yml
  format: yaml
  label: Refinitiv Real-Time WebSocket API
  slug: refinitiv-real-time-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/asyncapi/refinitiv-real-time-websocket-asyncapi.yml
- filename: refinitiv-datascope-select-openapi.yml
  format: yaml
  label: LSEG DataScope Select - REST API
  slug: lseg-datascope-select-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/openapi/refinitiv-datascope-select-openapi.yml
- filename: refinitiv-world-check-one-openapi.yml
  format: yaml
  label: World-Check One API
  slug: world-check-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/openapi/refinitiv-world-check-one-openapi.yml
- filename: refinitiv-qual-id-openapi.yml
  format: yaml
  label: Qual-ID API
  slug: qual-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/openapi/refinitiv-qual-id-openapi.yml
- filename: refinitiv-permid-entity-search-openapi.yml
  format: yaml
  label: PermID Entity Search API
  slug: permid-entity-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/openapi/refinitiv-permid-entity-search-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lseg.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: refinitiv.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: developers.lseg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  6 23:59:59 2027 GMT
  host: www.lseg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.refinitiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Refinitiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refinitiv, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Refinitiv
provider_slug: refinitiv
slug: refinitiv-domain-security
source_filename: refinitiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.lseg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.lseg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.refinitiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lseg.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: refinitiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/security/refinitiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags: []
---
