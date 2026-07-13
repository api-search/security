---
api_specs:
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Live Vessel Tracking API
  slug: datalastic-live-vessel-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Vessel Traffic in Radius API
  slug: datalastic-vessel-traffic-in-radius-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Historical Vessel Track API
  slug: datalastic-historical-vessel-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Vessel Info and Finder API
  slug: datalastic-vessel-info-and-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Port Finder API
  slug: datalastic-port-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
- filename: datalastic-openapi.yml
  format: yaml
  label: Datalastic Reports and Usage API
  slug: datalastic-reports-and-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/openapi/datalastic-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datalastic.com
  spf: true
hosts:
- cert_expires: Aug 23 18:02:35 2026 GMT
  host: datalastic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:50:43 2026 GMT
  host: api.datalastic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datalastic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datalastic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Datalastic
provider_slug: datalastic
slug: datalastic-domain-security
source_filename: datalastic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datalastic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:02:35 2026 GMT\n  hsts: false\n- host: api.datalastic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:50:43 2026 GMT\n  hsts: false\ndomains:\n- domain: datalastic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datalastic/refs/heads/main/security/datalastic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Vessel Tracking
- Maritime
- AIS
- Ships
- Ports
- Shipping
---
