---
api_specs:
- filename: spacex-api-openapi.yml
  format: yaml
  label: SpaceX API
  slug: spacex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/openapi/spacex-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spacex.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: spacexdata.com
  spf: false
hosts:
- cert_expires: Aug 20 11:21:47 2026 GMT
  host: www.spacex.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 22:27:28 2026 GMT
  host: api.spacexdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spacex Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpaceX API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SpaceX API
provider_slug: spacex-api
slug: spacex-api-domain-security
source_filename: spacex-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spacex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 11:21:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.spacexdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:27:28 2026 GMT\n  hsts: null\ndomains:\n- domain: spacex.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: spacexdata.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacex-api/refs/heads/main/security/spacex-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Space
- Aerospace
- Launches
- SpaceX
---
