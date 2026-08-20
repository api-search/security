---
api_specs:
- filename: mntn-ptv-advertisers-openapi.yml
  format: yaml
  label: MNTN Performance TV (PTV) API
  slug: mntn-performance-tv-ptv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-ptv-advertisers-openapi.yml
- filename: mntn-reporting-api-openapi.yml
  format: yaml
  label: MNTN Reporting API 3.0
  slug: mntn-reporting-api-30
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-reporting-api-openapi.yml
- filename: mntn-batch-export-openapi.yml
  format: yaml
  label: MNTN Async Batch Export API
  slug: mntn-async-batch-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-batch-export-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mountain.com
  spf: true
hosts:
- cert_expires: Nov  2 05:12:47 2026 GMT
  host: mountain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 13:40:36 2026 GMT
  host: api.mountain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 13:11:32 2026 GMT
  host: api3.mountain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mntn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MNTN, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MNTN
provider_slug: mntn
slug: mntn-domain-security
source_filename: mntn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mountain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 05:12:47 2026 GMT\n  hsts: false\n- host: api.mountain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:40:36 2026 GMT\n  hsts: null\n- host: api3.mountain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 13:11:32 2026 GMT\n  hsts: null\ndomains:\n- domain: mountain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/security/mntn-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Connected TV
- ctv-advertising
- Advertising
- Performance Marketing
- Streaming TV
- Media Buying
- Attribution
- Audience Targeting
- Conversion Tracking
- Programmatic Advertising
- private-marketplace
- marketing-reporting
- AdTech
---
