---
api_specs:
- filename: campaigns-api-openapi.yaml
  format: yaml
  label: MediaMath Campaigns V2.0 API
  slug: mediamath-campaigns-v20-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediamath/refs/heads/main/openapi/campaigns-api-openapi.yaml
- filename: reporting-api-openapi.yaml
  format: yaml
  label: MediaMath Reporting API V2
  slug: mediamath-reporting-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediamath/refs/heads/main/openapi/reporting-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mediamath.com
  spf: true
hosts:
- cert_expires: Sep 27 03:56:44 2026 GMT
  host: apidocs.mediamath.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.mediamath.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: ingest-default.prod.octane.mediamath.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mediamath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MediaMath, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MediaMath
provider_slug: mediamath
slug: mediamath-domain-security
source_filename: mediamath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apidocs.mediamath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 03:56:44 2026 GMT\n  hsts: false\n- host: api.mediamath.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\n- host: ingest-default.prod.octane.mediamath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mediamath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediamath/refs/heads/main/security/mediamath-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Programmatic Advertising
- DSP
- Demand-Side Platform
- Campaign Management
- Ad Tech
- Bidding
- Audience Segments
- Creative Management
- Reporting
- Analytics
---
