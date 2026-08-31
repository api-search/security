---
api_specs:
- filename: mntn-reporting-api-openapi.yml
  format: yaml
  label: MNTN Reporting API 3.0
  slug: mntn-reporting-api-30
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-reporting-api-openapi.yml
- filename: mntn-advertisers-api-openapi.yml
  format: yaml
  label: MNTN Advertisers API
  slug: mntn-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-advertisers-api-openapi.yml
- filename: mntn-api-api-openapi.yml
  format: yaml
  label: MNTN API
  slug: mntn-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-api-api-openapi.yml
- filename: mntn-attribution-api-openapi.yml
  format: yaml
  label: MNTN Attribution API
  slug: mntn-attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-attribution-api-openapi.yml
- filename: mntn-audiences-api-openapi.yml
  format: yaml
  label: MNTN Audiences API
  slug: mntn-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-audiences-api-openapi.yml
- filename: mntn-batch-api-openapi.yml
  format: yaml
  label: MNTN Batch API
  slug: mntn-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-batch-api-openapi.yml
- filename: mntn-campaigns-api-openapi.yml
  format: yaml
  label: MNTN Campaigns API
  slug: mntn-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-campaigns-api-openapi.yml
- filename: mntn-creatives-api-openapi.yml
  format: yaml
  label: MNTN Creatives API
  slug: mntn-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-creatives-api-openapi.yml
- filename: mntn-flights-api-openapi.yml
  format: yaml
  label: MNTN Flights API
  slug: mntn-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-flights-api-openapi.yml
- filename: mntn-organizations-api-openapi.yml
  format: yaml
  label: MNTN Organizations API
  slug: mntn-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-organizations-api-openapi.yml
- filename: mntn-pixel-api-openapi.yml
  format: yaml
  label: MNTN Pixel API
  slug: mntn-pixel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pixel-api-openapi.yml
- filename: mntn-pmp-campaign-deals-api-openapi.yml
  format: yaml
  label: MNTN Pmp Campaign Deals API
  slug: mntn-pmp-campaign-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pmp-campaign-deals-api-openapi.yml
- filename: mntn-pmp-channels-api-openapi.yml
  format: yaml
  label: MNTN Pmp Channels API
  slug: mntn-pmp-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pmp-channels-api-openapi.yml
- filename: mntn-pmp-deal-groups-api-openapi.yml
  format: yaml
  label: MNTN Pmp Deal Groups API
  slug: mntn-pmp-deal-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pmp-deal-groups-api-openapi.yml
- filename: mntn-pmp-deals-api-openapi.yml
  format: yaml
  label: MNTN Pmp Deals API
  slug: mntn-pmp-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pmp-deals-api-openapi.yml
- filename: mntn-pmp-partners-api-openapi.yml
  format: yaml
  label: MNTN Pmp Partners API
  slug: mntn-pmp-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pmp-partners-api-openapi.yml
- filename: mntn-reference-api-openapi.yml
  format: yaml
  label: MNTN Reference API
  slug: mntn-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-reference-api-openapi.yml
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
