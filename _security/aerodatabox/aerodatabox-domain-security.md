---
api_specs:
- filename: aerodatabox-aircraft-api-api-openapi.yml
  format: yaml
  label: AeroDataBox Aircraft API API
  slug: aerodatabox-aircraft-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-aircraft-api-api-openapi.yml
- filename: aerodatabox-airport-api-api-openapi.yml
  format: yaml
  label: AeroDataBox Airport API API
  slug: aerodatabox-airport-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-airport-api-api-openapi.yml
- filename: aerodatabox-flight-alert-api-api-openapi.yml
  format: yaml
  label: AeroDataBox Flight Alert API API
  slug: aerodatabox-flight-alert-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-flight-alert-api-api-openapi.yml
- filename: aerodatabox-flight-api-api-openapi.yml
  format: yaml
  label: AeroDataBox Flight API API
  slug: aerodatabox-flight-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-flight-api-api-openapi.yml
- filename: aerodatabox-healthcheck-api-api-openapi.yml
  format: yaml
  label: AeroDataBox Healthcheck API API
  slug: aerodatabox-healthcheck-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-healthcheck-api-api-openapi.yml
- filename: aerodatabox-industry-api-api-openapi.yml
  format: yaml
  label: AeroDataBox Industry API API
  slug: aerodatabox-industry-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-industry-api-api-openapi.yml
- filename: aerodatabox-miscellaneous-api-api-openapi.yml
  format: yaml
  label: AeroDataBox Miscellaneous API API
  slug: aerodatabox-miscellaneous-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-miscellaneous-api-api-openapi.yml
- filename: aerodatabox-statistical-api-api-openapi.yml
  format: yaml
  label: AeroDataBox Statistical API API
  slug: aerodatabox-statistical-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/openapi/aerodatabox-statistical-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aerodatabox.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: api.market
  spf: true
hosts:
- cert_expires: Sep  9 09:18:09 2026 GMT
  host: www.aerodatabox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 09:18:09 2026 GMT
  host: doc.aerodatabox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 00:28:08 2026 GMT
  host: prod.api.market
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aerodatabox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AeroDataBox, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AeroDataBox
provider_slug: aerodatabox
slug: aerodatabox-domain-security
source_filename: aerodatabox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aerodatabox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 09:18:09 2026 GMT\n  hsts: false\n- host: doc.aerodatabox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 09:18:09 2026 GMT\n  hsts: false\n- host: prod.api.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 00:28:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aerodatabox.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: api.market\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/security/aerodatabox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
---
