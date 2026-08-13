---
api_specs:
- filename: groundtruth-ads-manager-openapi.yml
  format: yaml
  label: GroundTruth Ads Manager Public API
  slug: groundtruth-ads-manager-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groundtruth/refs/heads/main/openapi/groundtruth-ads-manager-openapi.yml
- filename: groundtruth-reporting-openapi.yml
  format: yaml
  label: Groundtruth Reporting API
  slug: groundtruth-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groundtruth/refs/heads/main/openapi/groundtruth-reporting-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: groundtruth.com
  spf: true
hosts:
- cert_expires: Sep 30 11:19:44 2026 GMT
  host: www.groundtruth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 00:02:52 2026 GMT
  host: api-docs.groundtruth.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: api-public.groundtruth.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Groundtruth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GroundTruth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GroundTruth
provider_slug: groundtruth
slug: groundtruth-domain-security
source_filename: groundtruth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.groundtruth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 11:19:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-docs.groundtruth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  2 00:02:52 2026 GMT\n  hsts: false\n- host: api-public.groundtruth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: groundtruth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groundtruth/refs/heads/main/security/groundtruth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Martech
- Advertising
- Location Intelligence
- Marketing
- Adtech
- Location-Based Marketing
- Advertising API
- Campaign Management
- Ad Reporting
- Attribution
- Geofencing
- Digital Out Of Home
- CTV
---
