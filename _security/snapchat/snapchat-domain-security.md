---
api_specs:
- filename: snapchat-ads-api-openapi.yml
  format: yaml
  label: Snapchat Ads API
  slug: snapchat-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ads-api-openapi.yml
- filename: snapchat-ad-accounts-api-openapi.yml
  format: yaml
  label: Snapchat Ad Accounts API
  slug: snapchat-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ad-accounts-api-openapi.yml
- filename: snapchat-ad-squads-api-openapi.yml
  format: yaml
  label: Snapchat Ad Squads API
  slug: snapchat-ad-squads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ad-squads-api-openapi.yml
- filename: snapchat-audience-segments-api-openapi.yml
  format: yaml
  label: Snapchat Audience Segments API
  slug: snapchat-audience-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-audience-segments-api-openapi.yml
- filename: snapchat-campaigns-api-openapi.yml
  format: yaml
  label: Snapchat Campaigns API
  slug: snapchat-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-campaigns-api-openapi.yml
- filename: snapchat-conversion-events-api-openapi.yml
  format: yaml
  label: Snapchat Conversion Events API
  slug: snapchat-conversion-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-conversion-events-api-openapi.yml
- filename: snapchat-creatives-api-openapi.yml
  format: yaml
  label: Snapchat Creatives API
  slug: snapchat-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-creatives-api-openapi.yml
- filename: snapchat-funding-sources-api-openapi.yml
  format: yaml
  label: Snapchat Funding Sources API
  slug: snapchat-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-funding-sources-api-openapi.yml
- filename: snapchat-measurement-api-openapi.yml
  format: yaml
  label: Snapchat Measurement API
  slug: snapchat-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-measurement-api-openapi.yml
- filename: snapchat-media-api-openapi.yml
  format: yaml
  label: Snapchat Media API
  slug: snapchat-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-media-api-openapi.yml
- filename: snapchat-oauth-api-openapi.yml
  format: yaml
  label: Snapchat OAuth API
  slug: snapchat-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-oauth-api-openapi.yml
- filename: snapchat-organizations-api-openapi.yml
  format: yaml
  label: Snapchat Organizations API
  slug: snapchat-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-organizations-api-openapi.yml
- filename: snapchat-user-profile-api-openapi.yml
  format: yaml
  label: Snapchat User Profile API
  slug: snapchat-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-user-profile-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snap.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: snapchat.com
  spf: true
hosts:
- cert_expires: Oct 19 15:35:05 2026 GMT
  host: snap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 14:58:31 2026 GMT
  host: developers.snap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: adsapi.snapchat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snapchat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snapchat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Snapchat
provider_slug: snapchat
slug: snapchat-domain-security
source_filename: snapchat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 15:35:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.snap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 14:58:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: adsapi.snapchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: snap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: snapchat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/security/snapchat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- AR
- Augmented Reality
- Marketing
- Messaging
- Social-Media
---
