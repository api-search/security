---
api_specs:
- filename: artemis-apod-api-openapi.yml
  format: yaml
  label: Artemis APOD API
  slug: artemis-apod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-apod-api-openapi.yml
- filename: artemis-donki-api-openapi.yml
  format: yaml
  label: Artemis DONKI API
  slug: artemis-donki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-donki-api-openapi.yml
- filename: artemis-epic-api-openapi.yml
  format: yaml
  label: Artemis EPIC API
  slug: artemis-epic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-epic-api-openapi.yml
- filename: artemis-images-api-openapi.yml
  format: yaml
  label: Artemis Images API
  slug: artemis-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-images-api-openapi.yml
- filename: artemis-neows-api-openapi.yml
  format: yaml
  label: Artemis NeoWs API
  slug: artemis-neows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-neows-api-openapi.yml
- filename: artemis-techport-swagger.json
  format: json
  label: NASA TechPort API
  slug: nasa-techport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-techport-swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nasa.gov
  spf: true
hosts:
- cert_expires: Nov  9 23:22:58 2026 GMT
  host: www.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 19:21:05 2026 GMT
  host: api.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: technology.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Artemis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artemis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Artemis
provider_slug: artemis
slug: artemis-domain-security
source_filename: artemis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:22:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 19:21:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: technology.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/security/artemis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Exploration
- Lunar
- Moon
- NASA
- Space
- Government
---
