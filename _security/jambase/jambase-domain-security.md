---
api_specs:
- filename: jambase-artists-api-openapi.yml
  format: yaml
  label: JamBase Artists API
  slug: jambase-artists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jambase/refs/heads/main/openapi/jambase-artists-api-openapi.yml
- filename: jambase-events-api-openapi.yml
  format: yaml
  label: JamBase Events API
  slug: jambase-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jambase/refs/heads/main/openapi/jambase-events-api-openapi.yml
- filename: jambase-genres-api-openapi.yml
  format: yaml
  label: JamBase Genres API
  slug: jambase-genres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jambase/refs/heads/main/openapi/jambase-genres-api-openapi.yml
- filename: jambase-geographies-api-openapi.yml
  format: yaml
  label: JamBase Geographies API
  slug: jambase-geographies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jambase/refs/heads/main/openapi/jambase-geographies-api-openapi.yml
- filename: jambase-lookups-api-openapi.yml
  format: yaml
  label: JamBase Lookups API
  slug: jambase-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jambase/refs/heads/main/openapi/jambase-lookups-api-openapi.yml
- filename: jambase-streams-api-openapi.yml
  format: yaml
  label: JamBase Streams API
  slug: jambase-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jambase/refs/heads/main/openapi/jambase-streams-api-openapi.yml
- filename: jambase-venues-api-openapi.yml
  format: yaml
  label: JamBase Venues API
  slug: jambase-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jambase/refs/heads/main/openapi/jambase-venues-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jambase.com
  spf: true
hosts:
- cert_expires: Sep  6 20:19:16 2026 GMT
  host: data.jambase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 10:30:52 2026 GMT
  host: www.jambase.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 16:31:03 2026 GMT
  host: api.data.jambase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jambase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JamBase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JamBase
provider_slug: jambase
slug: jambase-domain-security
source_filename: jambase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.jambase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 20:19:16 2026 GMT\n  hsts: false\n- host: www.jambase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 10:30:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.data.jambase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 16:31:03 2026 GMT\n  hsts: null\ndomains:\n- domain: jambase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jambase/refs/heads/main/security/jambase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artists
- Concerts
- Event
- Festivals
- Live Music
- Music
- Setlists
- Tickets
- Tours
- Venues
---
