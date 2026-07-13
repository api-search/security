---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@here.com"
  - 0 issue "amazon.com"
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
- cert_expires: Aug 25 12:16:15 2026 GMT
  host: www.here.com
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
  host: autosuggest.search.hereapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Here Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HERE Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HERE Technologies
provider_slug: here-technologies
slug: here-technologies-domain-security
source_filename: here-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.here.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:16:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: geocode.search.hereapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 08:36:15 2026 GMT\n  hsts: null\n- host: autosuggest.search.hereapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 08:36:15 2026 GMT\n  hsts: null\ndomains:\n- domain: here.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@here.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hereapi.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 iodef \"mailto:security@here.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/here-technologies/refs/heads/main/security/here-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Maps
- Geocoding
- Routing
- Location Services
- Traffic
- HD Live Map
- Automotive
- Fleet
---
