---
api_specs:
- filename: metro-transit-nextrip-openapi.json
  format: json
  label: Metro Transit NexTrip API
  slug: nextrip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-transit/refs/heads/main/openapi/metro-transit-nextrip-openapi.json
- filename: metro-transit-alerts-openapi.json
  format: json
  label: Metro Transit Service Alerts API
  slug: alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-transit/refs/heads/main/openapi/metro-transit-alerts-openapi.json
- filename: metro-transit-tripplanner-openapi.json
  format: json
  label: Metro Transit Trip Planner API
  slug: trip-planner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-transit/refs/heads/main/openapi/metro-transit-tripplanner-openapi.json
- filename: metro-transit-schedule-openapi.json
  format: json
  label: Metro Transit Schedule API
  slug: schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-transit/refs/heads/main/openapi/metro-transit-schedule-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metrotransit.org
  spf: true
hosts:
- cert_expires: Oct  1 05:18:25 2026 GMT
  host: www.metrotransit.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: svc.metrotransit.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metro Transit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metro Transit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Metro Transit
provider_slug: metro-transit
slug: metro-transit-domain-security
source_filename: metro-transit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metrotransit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:18:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: svc.metrotransit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: metrotransit.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metro-transit/refs/heads/main/security/metro-transit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Minneapolis
- Minnesota
- Public Transportation
- Real-Time
- Transit
---
