---
api_specs:
- filename: fleetmon-openapi.yml
  format: yaml
  label: FleetMon Vessels API (Retired)
  slug: fleetmon-vessels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetmon/refs/heads/main/openapi/fleetmon-openapi.yml
- filename: fleetmon-openapi.yml
  format: yaml
  label: FleetMon Vessel Positions API (Retired)
  slug: fleetmon-vessel-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetmon/refs/heads/main/openapi/fleetmon-openapi.yml
- filename: fleetmon-openapi.yml
  format: yaml
  label: FleetMon Port Calls & ETA API (Retired)
  slug: fleetmon-port-calls-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetmon/refs/heads/main/openapi/fleetmon-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kpler.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archive.org
  spf: true
hosts:
- cert_expires: Aug 22 02:44:31 2026 GMT
  host: www.kpler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 22:02:42 2027 GMT
  host: web.archive.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: apiv2.fleetmon.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fleetmon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FleetMon, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FleetMon
provider_slug: fleetmon
slug: fleetmon-domain-security
source_filename: fleetmon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kpler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:44:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: web.archive.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 22:02:42 2027 GMT\n  hsts: false\n- host: apiv2.fleetmon.com\n  https: false\ndomains:\n- domain: kpler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: archive.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleetmon/refs/heads/main/security/fleetmon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vessel Tracking
- Maritime
- AIS
- Ships
- Ports
- Port Calls
- Shipping
- Retired
---
