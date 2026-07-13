---
api_specs:
- filename: sound-transit-onebusaway-openapi.yml
  format: yaml
  label: Sound Transit OneBusAway API
  slug: sound-transit-onebusaway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sound-transit/refs/heads/main/openapi/sound-transit-onebusaway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: soundtransit.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onebusaway.org
  spf: true
hosts:
- cert_expires: Sep 27 11:28:57 2026 GMT
  host: www.soundtransit.org
  hsts: true
  hsts_max_age: 31557600
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
name: Sound Transit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sound Transit, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sound Transit
provider_slug: sound-transit
slug: sound-transit-domain-security
source_filename: sound-transit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soundtransit.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 11:28:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.pugetsound.onebusaway.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: soundtransit.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: onebusaway.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sound-transit/refs/heads/main/security/sound-transit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transit
- Transportation
- GTFS
- Real-Time
- Public Transit
- Government
- Seattle
---
