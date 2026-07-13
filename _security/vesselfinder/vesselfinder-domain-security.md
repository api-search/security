---
api_specs:
- filename: vesselfinder-ais-api-openapi.yml
  format: yaml
  label: VesselFinder AIS API
  slug: vesselfinder-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-ais-api-openapi.yml
- filename: vesselfinder-container-tracking-api-openapi.yml
  format: yaml
  label: VesselFinder Container Tracking API
  slug: vesselfinder-container-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-container-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vesselfinder.com
  spf: true
hosts:
- cert_expires: Aug 16 20:33:05 2026 GMT
  host: www.vesselfinder.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 20:33:05 2026 GMT
  host: api.vesselfinder.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 20:33:05 2026 GMT
  host: container.vesselfinder.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vesselfinder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VesselFinder, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VesselFinder
provider_slug: vesselfinder
slug: vesselfinder-domain-security
source_filename: vesselfinder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vesselfinder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:33:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vesselfinder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:33:05 2026 GMT\n  hsts: false\n- host: container.vesselfinder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:33:05 2026 GMT\n  hsts: false\ndomains:\n- domain: vesselfinder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/security/vesselfinder-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AIS
- Maritime
- Vessel Tracking
- Container Tracking
- Geospatial
- Logistics
- Ports
- Supply Chain
---
