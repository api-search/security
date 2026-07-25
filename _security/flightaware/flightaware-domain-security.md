---
api_specs:
- filename: flightaware-airports-api-openapi.yml
  format: yaml
  label: FlightAware airports API
  slug: flightaware-airports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-airports-api-openapi.yml
- filename: flightaware-alerts-api-openapi.yml
  format: yaml
  label: FlightAware alerts API
  slug: flightaware-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-alerts-api-openapi.yml
- filename: flightaware-flights-api-openapi.yml
  format: yaml
  label: FlightAware flights API
  slug: flightaware-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-flights-api-openapi.yml
- filename: flightaware-foresight-api-openapi.yml
  format: yaml
  label: FlightAware foresight API
  slug: flightaware-foresight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-foresight-api-openapi.yml
- filename: flightaware-history-api-openapi.yml
  format: yaml
  label: FlightAware history API
  slug: flightaware-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-history-api-openapi.yml
- filename: flightaware-miscellaneous-api-openapi.yml
  format: yaml
  label: FlightAware miscellaneous API
  slug: flightaware-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-miscellaneous-api-openapi.yml
- filename: flightaware-operators-api-openapi.yml
  format: yaml
  label: FlightAware operators API
  slug: flightaware-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/openapi/flightaware-operators-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: flightaware.com
  spf: true
hosts:
- cert_expires: Aug 14 00:51:13 2026 GMT
  host: www.flightaware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 15:23:27 2027 GMT
  host: aeroapi.flightaware.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Flightaware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlightAware, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: FlightAware
provider_slug: flightaware
slug: flightaware-domain-security
source_filename: flightaware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flightaware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 00:51:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: aeroapi.flightaware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 16 15:23:27 2027 GMT\n  hsts: null\ndomains:\n- domain: flightaware.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightaware/refs/heads/main/security/flightaware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Aviation
- Flights
- Flight Tracking
- Mapping
- Radar
- Satellites
- Traffic Control
---
