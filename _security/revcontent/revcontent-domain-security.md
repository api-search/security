---
api_specs:
- filename: revcontent-access-api-openapi.yml
  format: yaml
  label: RevContent Access API
  slug: revcontent-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-access-api-openapi.yml
- filename: revcontent-ccpa-api-openapi.yml
  format: yaml
  label: RevContent CCPA API
  slug: revcontent-ccpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-ccpa-api-openapi.yml
- filename: revcontent-content-api-openapi.yml
  format: yaml
  label: RevContent Content API
  slug: revcontent-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-content-api-openapi.yml
- filename: revcontent-conversions-api-openapi.yml
  format: yaml
  label: RevContent Conversions API
  slug: revcontent-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-conversions-api-openapi.yml
- filename: revcontent-helpers-api-openapi.yml
  format: yaml
  label: RevContent Helpers API
  slug: revcontent-helpers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-helpers-api-openapi.yml
- filename: revcontent-sub-accounts-api-openapi.yml
  format: yaml
  label: RevContent Sub Accounts API
  slug: revcontent-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-sub-accounts-api-openapi.yml
- filename: revcontent-targeting-api-openapi.yml
  format: yaml
  label: RevContent Targeting API
  slug: revcontent-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-targeting-api-openapi.yml
- filename: revcontent-widget-internal-content-api-openapi.yml
  format: yaml
  label: RevContent Widget Internal Content API
  slug: revcontent-widget-internal-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widget-internal-content-api-openapi.yml
- filename: revcontent-widget-optimizer-api-openapi.yml
  format: yaml
  label: RevContent Widget Optimizer API
  slug: revcontent-widget-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widget-optimizer-api-openapi.yml
- filename: revcontent-campaigns-api-openapi.yml
  format: yaml
  label: RevContent Campaigns API
  slug: revcontent-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-campaigns-api-openapi.yml
- filename: revcontent-widget-api-openapi.yml
  format: yaml
  label: RevContent Widget API
  slug: revcontent-widget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/openapi/revcontent-widget-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: revcontent.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: revcontent.io
  spf: false
hosts:
- cert_expires: Sep 18 13:55:39 2026 GMT
  host: www.revcontent.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 07:43:47 2026 GMT
  host: help.revcontent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 13:55:39 2026 GMT
  host: api.revcontent.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revcontent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RevContent, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RevContent
provider_slug: revcontent
slug: revcontent-domain-security
source_filename: revcontent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revcontent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:55:39 2026 GMT\n  hsts: false\n- host: help.revcontent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:43:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.revcontent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:55:39 2026 GMT\n  hsts: false\ndomains:\n- domain: revcontent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: revcontent.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revcontent/refs/heads/main/security/revcontent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Native Advertising
- Content Recommendation
- Ad Network
- Publisher Monetization
- Programmatic Advertising
- Advertising Technology
- Campaign Management
- Audience Targeting
- Conversion Tracking
- Marketing
---
