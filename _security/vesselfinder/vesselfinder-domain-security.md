---
api_specs:
- filename: vesselfinder-containers-api-openapi.yml
  format: yaml
  label: VesselFinder Containers API
  slug: vesselfinder-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-containers-api-openapi.yml
- filename: vesselfinder-distance-api-openapi.yml
  format: yaml
  label: VesselFinder Distance API
  slug: vesselfinder-distance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-distance-api-openapi.yml
- filename: vesselfinder-expected-arrivals-api-openapi.yml
  format: yaml
  label: VesselFinder Expected Arrivals API
  slug: vesselfinder-expected-arrivals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-expected-arrivals-api-openapi.yml
- filename: vesselfinder-list-manager-api-openapi.yml
  format: yaml
  label: VesselFinder List Manager API
  slug: vesselfinder-list-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-list-manager-api-openapi.yml
- filename: vesselfinder-live-data-api-openapi.yml
  format: yaml
  label: VesselFinder Live Data API
  slug: vesselfinder-live-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-live-data-api-openapi.yml
- filename: vesselfinder-master-data-api-openapi.yml
  format: yaml
  label: VesselFinder Master Data API
  slug: vesselfinder-master-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-master-data-api-openapi.yml
- filename: vesselfinder-port-calls-api-openapi.yml
  format: yaml
  label: VesselFinder Port Calls API
  slug: vesselfinder-port-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-port-calls-api-openapi.yml
- filename: vesselfinder-status-api-openapi.yml
  format: yaml
  label: VesselFinder Status API
  slug: vesselfinder-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-status-api-openapi.yml
- filename: vesselfinder-vessels-api-openapi.yml
  format: yaml
  label: VesselFinder Vessels API
  slug: vesselfinder-vessels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-vessels-api-openapi.yml
- filename: vesselfinder-vessels-list-api-openapi.yml
  format: yaml
  label: VesselFinder Vessels List API
  slug: vesselfinder-vessels-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-vessels-list-api-openapi.yml
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
