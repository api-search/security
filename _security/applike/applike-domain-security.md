---
api_specs:
- filename: applike-app-partner-connection-api-openapi.yml
  format: yaml
  label: AppLike Group App Partner Connection API
  slug: applike-app-partner-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-app-partner-connection-api-openapi.yml
- filename: applike-appevents-api-openapi.yml
  format: yaml
  label: AppLike Group Appevents API
  slug: applike-appevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-appevents-api-openapi.yml
- filename: applike-apps-api-openapi.yml
  format: yaml
  label: AppLike Group Apps API
  slug: applike-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-apps-api-openapi.yml
- filename: applike-bids-api-openapi.yml
  format: yaml
  label: AppLike Group Bids API
  slug: applike-bids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-bids-api-openapi.yml
- filename: applike-campaigns-api-openapi.yml
  format: yaml
  label: AppLike Group Campaigns API
  slug: applike-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-campaigns-api-openapi.yml
- filename: applike-partner-configurations-api-openapi.yml
  format: yaml
  label: AppLike Group Partner Configurations API
  slug: applike-partner-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-partner-configurations-api-openapi.yml
- filename: applike-partners-api-openapi.yml
  format: yaml
  label: AppLike Group Partners API
  slug: applike-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/openapi/applike-partners-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: applike-group.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: justtrack.io
  spf: true
hosts:
- cert_expires: Nov  1 13:55:23 2026 GMT
  host: applike-group.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: docs.justtrack.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.justtrack.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Applike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppLike Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AppLike Group
provider_slug: applike
slug: applike-domain-security
source_filename: applike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: applike-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 13:55:23 2026 GMT\n  hsts: false\n- host: docs.justtrack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.justtrack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: applike-group.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: justtrack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applike/refs/heads/main/security/applike-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Mobile Attribution
- User Acquisition
- AdTech
- Mobile Advertising
- App Monetization
- rewarded-advertising
- Mobile SDK
- Mobile Analytics
- Marketing Attribution
- Mobile Games
- Event Tracking
- Company
---
