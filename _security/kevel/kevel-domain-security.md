---
api_specs:
- filename: kevel-ads-api-openapi.yml
  format: yaml
  label: Kevel Ads API
  slug: kevel-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-ads-api-openapi.yml
- filename: kevel-advertisers-api-openapi.yml
  format: yaml
  label: Kevel Advertisers API
  slug: kevel-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-advertisers-api-openapi.yml
- filename: kevel-campaigns-api-openapi.yml
  format: yaml
  label: Kevel Campaigns API
  slug: kevel-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-campaigns-api-openapi.yml
- filename: kevel-channels-api-openapi.yml
  format: yaml
  label: Kevel Channels API
  slug: kevel-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-channels-api-openapi.yml
- filename: kevel-creatives-api-openapi.yml
  format: yaml
  label: Kevel Creatives API
  slug: kevel-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-creatives-api-openapi.yml
- filename: kevel-decision-api-openapi.yml
  format: yaml
  label: Kevel Decision API
  slug: kevel-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-decision-api-openapi.yml
- filename: kevel-flights-api-openapi.yml
  format: yaml
  label: Kevel Flights API
  slug: kevel-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-flights-api-openapi.yml
- filename: kevel-reporting-api-openapi.yml
  format: yaml
  label: Kevel Reporting API
  slug: kevel-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-reporting-api-openapi.yml
- filename: kevel-sites-api-openapi.yml
  format: yaml
  label: Kevel Sites API
  slug: kevel-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-sites-api-openapi.yml
- filename: kevel-zones-api-openapi.yml
  format: yaml
  label: Kevel Zones API
  slug: kevel-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-zones-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kevel.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@kevel.co"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kevel.co
  spf: true
hosts:
- cert_expires: Aug 16 14:03:14 2026 GMT
  host: www.kevel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: dev.kevel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.kevel.co
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kevel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kevel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kevel
provider_slug: kevel
slug: kevel-domain-security
source_filename: kevel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kevel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 14:03:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.kevel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kevel.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: kevel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kevel.co\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@kevel.co\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/security/kevel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ad Serving
- Advertising
- API-First
- Audience
- Monetization
- Reporting
---
