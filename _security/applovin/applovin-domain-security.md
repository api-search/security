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
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: axon.ai
  spf: true
hosts:
- cert_expires: Aug 30 07:59:18 2026 GMT
  host: www.applovin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 07:48:25 2026 GMT
  host: support.axon.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:32:17 2026 GMT
  host: r.applovin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Applovin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppLovin, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AppLovin
provider_slug: applovin
slug: applovin-domain-security
source_filename: applovin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.applovin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 07:59:18 2026 GMT\n  hsts: false\n- host: support.axon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:48:25 2026 GMT\n  hsts: false\n- host: r.applovin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:32:17 2026 GMT\n  hsts: null\ndomains:\n- domain: applovin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: axon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/security/applovin-domain-security.yml
summary_line: TLSv1.3 · DMARC
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
