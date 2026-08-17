---
api_specs:
- filename: applovin-ad-units-api-openapi.yml
  format: yaml
  label: AppLovin Ad Units API
  slug: applovin-ad-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-ad-units-api-openapi.yml
- filename: applovin-asset-reporting-api-openapi.yml
  format: yaml
  label: AppLovin Asset Reporting API
  slug: applovin-asset-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-asset-reporting-api-openapi.yml
- filename: applovin-assets-api-openapi.yml
  format: yaml
  label: AppLovin Assets API
  slug: applovin-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-assets-api-openapi.yml
- filename: applovin-campaigns-api-openapi.yml
  format: yaml
  label: AppLovin Campaigns API
  slug: applovin-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-campaigns-api-openapi.yml
- filename: applovin-conversion-events-api-openapi.yml
  format: yaml
  label: AppLovin Conversion Events API
  slug: applovin-conversion-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-conversion-events-api-openapi.yml
- filename: applovin-creative-sets-api-openapi.yml
  format: yaml
  label: AppLovin Creative Sets API
  slug: applovin-creative-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-creative-sets-api-openapi.yml
- filename: applovin-experiments-api-openapi.yml
  format: yaml
  label: AppLovin Experiments API
  slug: applovin-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-experiments-api-openapi.yml
- filename: applovin-growth-reporting-api-openapi.yml
  format: yaml
  label: AppLovin Growth Reporting API
  slug: applovin-growth-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-growth-reporting-api-openapi.yml
- filename: applovin-revenue-reporting-api-openapi.yml
  format: yaml
  label: AppLovin Revenue Reporting API
  slug: applovin-revenue-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-revenue-reporting-api-openapi.yml
- filename: applovin-test-devices-api-openapi.yml
  format: yaml
  label: AppLovin Test Devices API
  slug: applovin-test-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-test-devices-api-openapi.yml
- filename: applovin-waterfalls-api-openapi.yml
  format: yaml
  label: AppLovin Waterfalls API
  slug: applovin-waterfalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-waterfalls-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: applovin.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: axon.ai
  note: The axon.ai domain — which serves the Campaign Management API host and, until recently, the documentation — publishes no SPF and no DMARC record, unlike applovin.com which publishes both with p=reject. A brand AppLovin routes production API traffic through has materially weaker DNS-layer hygiene than its primary domain.
  spf: false
hosts:
- cert_expires: Oct 22 01:15:43 2026 GMT
  host: www.applovin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: Website
  tls_version: TLSv1.3
- cert_expires: Oct 19 17:17:28 2026 GMT
  host: support.applovin.com
  hsts: false
  https: true
  role: Documentation / DeveloperPortal
  tls_version: TLSv1.3
- cert_expires: Sep  1 22:30:27 2026 GMT
  host: max.applovin.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: Dashboard / SignUp (dash.applovin.com redirects here)
  root_status: 302
  tls_version: TLSv1.3
- cert_expires: Sep 28 05:29:31 2026 GMT
  host: o.applovin.com
  hsts: false
  https: true
  role: MAX Ad Unit Management API (baseURL)
  tls_version: TLSv1.3
- cert_expires: Oct 11 00:50:43 2026 GMT
  host: r.applovin.com
  hsts: false
  https: true
  note: Returns {"error":"Bad request"} for any unrouted path, including every /.well-known/ probe. This is also the host that accepts the Report Key as a query-string parameter.
  role: Reporting family (baseURL)
  root_status: 400
  tls_version: TLSv1.3
- cert_expires: Oct  5 05:04:46 2026 GMT
  host: b.applovin.com
  hsts: false
  https: true
  role: Conversion API (baseURL)
  root_status: 403
  tls_version: TLSv1.3
- cert_expires: Oct  5 07:03:36 2026 GMT
  host: api.ads.axon.ai
  hsts: false
  https: true
  role: Axon Campaign Management API (baseURL / OpenAPI servers[])
  root_status: 404
  server: nginx
  tls_version: TLSv1.3
- cert_expires: Oct 14 01:17:28 2026 GMT
  host: api-safedk.applovin.com
  hsts: false
  https: true
  role: Ad Review Rules Management API
  root_status: 200
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Applovin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppLovin, probed live across 8 host(s) and 2 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AppLovin
provider_slug: applovin
slug: applovin-domain-security
source_filename: applovin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every apis.yml baseURL host, every OpenAPI servers[] host, and the website/portal hosts\nnote: >-\n  Every AppLovin host negotiates TLS 1.3 with a valid certificate, and the applovin.com\n  domain publishes SPF and a DMARC policy of `reject` — the strongest email posture\n  available. The gaps are in the API layer: HSTS is set on the marketing site and the\n  dashboard but NOT on any of the four API hosts, there is no CAA record on either\n  registrable domain, and DNSSEC is not enabled on either. The four API hosts also carry\n  no /.well-known/ surface at all (see well-known/applovin-well-known.yml).\nhosts:\n- host: www.applovin.com\n  role: Website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct 22 01:15:43 2026 GMT'\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.applovin.com\n  role: Documentation / DeveloperPortal\n  https: true\n  tls_version: TLSv1.3\n  cert_expires:\
  \ 'Oct 19 17:17:28 2026 GMT'\n  hsts: false\n- host: max.applovin.com\n  role: Dashboard / SignUp (dash.applovin.com redirects here)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Sep  1 22:30:27 2026 GMT'\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  root_status: 302\n- host: o.applovin.com\n  role: MAX Ad Unit Management API (baseURL)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Sep 28 05:29:31 2026 GMT'\n  hsts: false\n- host: r.applovin.com\n  role: Reporting family (baseURL)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct 11 00:50:43 2026 GMT'\n  hsts: false\n  root_status: 400\n  note: >-\n    Returns {\"error\":\"Bad request\"} for any unrouted path, including every /.well-known/\n    probe. This is also the host that accepts the Report Key as a query-string parameter.\n- host: b.applovin.com\n  role: Conversion API (baseURL)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct  5 05:04:46 2026 GMT'\n  hsts:\
  \ false\n  root_status: 403\n- host: api.ads.axon.ai\n  role: Axon Campaign Management API (baseURL / OpenAPI servers[])\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct  5 07:03:36 2026 GMT'\n  hsts: false\n  root_status: 404\n  server: nginx\n- host: api-safedk.applovin.com\n  role: Ad Review Rules Management API\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: 'Oct 14 01:17:28 2026 GMT'\n  hsts: false\n  root_status: 200\ndomains:\n- domain: applovin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: axon.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: >-\n    The axon.ai domain — which serves the Campaign Management API host and, until recently,\n    the documentation — publishes no SPF and no DMARC record, unlike applovin.com which\n    publishes both with p=reject. A brand AppLovin routes production API traffic through\n    has materially weaker DNS-layer hygiene than its primary domain.\nfindings:\n\
  - {severity: info, finding: 'All eight hosts negotiate TLS 1.3 with valid certificates.'}\n- {severity: info, finding: 'applovin.com publishes SPF and DMARC p=reject.'}\n- {severity: low, finding: 'No HSTS on any of the four API hosts (o., r., b., api.ads.axon.ai) or on api-safedk.'}\n- {severity: low, finding: 'No CAA record on applovin.com or axon.ai — any CA may issue for either domain.'}\n- {severity: low, finding: 'DNSSEC not enabled on applovin.com or axon.ai.'}\n- {severity: medium, finding: 'axon.ai publishes neither SPF nor DMARC, while it serves a production API host.'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/security/applovin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Mobile
- AdTech
- App Monetization
- Mediation
- User Acquisition
- Marketing Technology
- Conversion Tracking
---
