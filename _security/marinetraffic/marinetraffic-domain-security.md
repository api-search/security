---
api_specs:
- filename: marinetraffic-ais-openapi.yml
  format: yaml
  label: MarineTraffic AIS Vessel Tracking API
  slug: marinetraffic-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/openapi/marinetraffic-ais-openapi.yml
- filename: marinetraffic-ais-openapi.yml
  format: yaml
  label: MarineTraffic AIS Vessel Tracking API
  slug: marinetraffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/openapi/marinetraffic-ais-openapi.yml
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
  dmarc_policy: quarantine
  dnssec: false
  domain: marinetraffic.com
  spf: true
hosts:
- cert_expires: Aug 22 02:44:31 2026 GMT
  host: www.kpler.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 18:34:35 2026 GMT
  host: services.marinetraffic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 18:34:35 2026 GMT
  host: www.marinetraffic.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marinetraffic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarineTraffic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MarineTraffic
provider_slug: marinetraffic
slug: marinetraffic-domain-security
source_filename: marinetraffic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kpler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:44:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.marinetraffic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:34:35 2026 GMT\n  hsts: null\n- host: www.marinetraffic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:34:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kpler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: marinetraffic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marinetraffic/refs/heads/main/security/marinetraffic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIS
- Maritime
- Shipping
- Vessel Tracking
---
