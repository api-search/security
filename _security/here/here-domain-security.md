---
api_specs:
- filename: here-apis-openapi.yml
  format: yaml
  label: HERE APIs
  slug: here-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here/refs/heads/main/properties/here-apis-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@here.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: here.com
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 iodef "mailto:security@here.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hereapi.com
  spf: true
hosts:
- cert_expires: Oct  9 20:16:08 2026 GMT
  host: developer.here.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 08:36:15 2026 GMT
  host: geocode.search.hereapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 08:36:15 2026 GMT
  host: discover.search.hereapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Here Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HERE, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HERE
provider_slug: here
slug: here-domain-security
source_filename: here-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.here.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 20:16:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: geocode.search.hereapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 08:36:15 2026 GMT\n  hsts: null\n- host: discover.search.hereapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 08:36:15 2026 GMT\n  hsts: null\ndomains:\n- domain: here.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@here.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hereapi.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 iodef \"mailto:security@here.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/here/refs/heads/main/security/here-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Location
- Mapping
- Maps
- Spatial
---
