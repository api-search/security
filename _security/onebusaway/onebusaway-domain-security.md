---
api_specs:
- filename: openapi.yml
  format: yaml
  label: OneBusAway REST API
  slug: onebusaway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/OneBusAway/sdk-config/main/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opentransitsoftwarefoundation.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onebusaway.org
  spf: true
hosts:
- cert_expires: Sep 24 04:45:00 2026 GMT
  host: opentransitsoftwarefoundation.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 18:00:26 2026 GMT
  host: developer.onebusaway.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: api.pugetsound.onebusaway.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onebusaway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneBusAway, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OneBusAway
provider_slug: onebusaway
slug: onebusaway-domain-security
source_filename: onebusaway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opentransitsoftwarefoundation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:45:00 2026 GMT\n  hsts: false\n- host: developer.onebusaway.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 18:00:26 2026 GMT\n  hsts: false\n- host: api.pugetsound.onebusaway.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: opentransitsoftwarefoundation.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: onebusaway.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onebusaway/refs/heads/main/security/onebusaway-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transit
- Public Transit
- Real-Time
- Arrivals
- Departures
- Bus
- GTFS
- Open Source
- Stop Data
- Trip Planning
- Service Alerts
- Vehicle Positions
- Open Data
---
