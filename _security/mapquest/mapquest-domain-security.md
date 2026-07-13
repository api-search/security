---
api_specs:
- filename: mapquest-openapi.yml
  format: yaml
  label: MapQuest Directions API
  slug: mapquest-directions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapquest/refs/heads/main/openapi/mapquest-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:devops@system1.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mapquest.com
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 iodef "mailto:devops@system1.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: mapquestapi.com
  spf: false
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: developer.mapquest.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: www.mapquestapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mapquest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MapQuest, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MapQuest
provider_slug: mapquest
slug: mapquest-domain-security
source_filename: mapquest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.mapquest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: www.mapquestapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mapquest.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:devops@system1.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: mapquestapi.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 iodef \"mailto:devops@system1.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mapquest/refs/heads/main/security/mapquest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- Mapping
- Maps
- Navigation
- Routing
- Traffic
---
