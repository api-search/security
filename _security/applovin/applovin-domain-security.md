---
api_specs:
- filename: applovin-max-revenue-reporting.yaml
  format: yaml
  label: AppLovin MAX Revenue Reporting API
  slug: applovin-max-revenue-reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-max-revenue-reporting.yaml
- filename: applovin-max-ad-unit-management.yaml
  format: yaml
  label: AppLovin MAX Ad Unit Management API
  slug: applovin-max-ad-unit-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-max-ad-unit-management.yaml
- filename: applovin-growth-reporting.yaml
  format: yaml
  label: AppLovin Growth (Axon / AppDiscovery) Reporting API
  slug: applovin-growth-reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-growth-reporting.yaml
- filename: applovin-growth-asset-reporting.yaml
  format: yaml
  label: AppLovin Growth Asset Reporting API
  slug: applovin-growth-asset-reporting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-growth-asset-reporting.yaml
- filename: applovin-axon-campaign-management.yaml
  format: yaml
  label: AppLovin Axon Campaign Management API
  slug: applovin-axon-campaign-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-axon-campaign-management.yaml
- filename: applovin-conversion-api-lead-gen.yaml
  format: yaml
  label: AppLovin Conversion API for Lead Generation
  slug: applovin-conversion-api-lead-gen
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-conversion-api-lead-gen.yaml
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
