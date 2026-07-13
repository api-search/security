---
api_specs:
- filename: nominatim-openapi.yml
  format: yaml
  label: Nominatim API
  slug: nominatim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nominatim/refs/heads/main/openapi/nominatim-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nominatim.org
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:hostmaster@openstreetmap.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openstreetmap.org
  spf: true
hosts:
- cert_expires: Aug 28 08:10:35 2026 GMT
  host: nominatim.org
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  7 06:40:06 2026 GMT
  host: nominatim.openstreetmap.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nominatim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nominatim, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nominatim
provider_slug: nominatim
slug: nominatim-domain-security
source_filename: nominatim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nominatim.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 28 08:10:35 2026 GMT\n  hsts: false\n- host: nominatim.openstreetmap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 06:40:06 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: nominatim.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openstreetmap.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:hostmaster@openstreetmap.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nominatim/refs/heads/main/security/nominatim-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Geocoding
- OpenStreetMap
- Maps
- LocationServices
- OpenSource
- Public APIs
---
