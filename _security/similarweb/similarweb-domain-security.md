---
api_specs:
- filename: similarweb-account-api-openapi.yml
  format: yaml
  label: SimilarWeb Account API
  slug: similarweb-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-account-api-openapi.yml
- filename: similarweb-app-intelligence-api-openapi.yml
  format: yaml
  label: SimilarWeb App Intelligence API
  slug: similarweb-app-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-app-intelligence-api-openapi.yml
- filename: similarweb-credits-api-openapi.yml
  format: yaml
  label: SimilarWeb Credits API
  slug: similarweb-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-credits-api-openapi.yml
- filename: similarweb-geography-api-openapi.yml
  format: yaml
  label: SimilarWeb Geography API
  slug: similarweb-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-geography-api-openapi.yml
- filename: similarweb-integrations-api-openapi.yml
  format: yaml
  label: SimilarWeb Integrations API
  slug: similarweb-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-integrations-api-openapi.yml
- filename: similarweb-keywords-api-openapi.yml
  format: yaml
  label: SimilarWeb Keywords API
  slug: similarweb-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-keywords-api-openapi.yml
- filename: similarweb-lead-enrichment-api-openapi.yml
  format: yaml
  label: SimilarWeb Lead Enrichment API
  slug: similarweb-lead-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-lead-enrichment-api-openapi.yml
- filename: similarweb-rankings-api-openapi.yml
  format: yaml
  label: SimilarWeb Rankings API
  slug: similarweb-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-rankings-api-openapi.yml
- filename: similarweb-reports-api-openapi.yml
  format: yaml
  label: SimilarWeb Reports API
  slug: similarweb-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-reports-api-openapi.yml
- filename: similarweb-similar-sites-api-openapi.yml
  format: yaml
  label: SimilarWeb Similar Sites API
  slug: similarweb-similar-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-similar-sites-api-openapi.yml
- filename: similarweb-traffic-and-engagement-api-openapi.yml
  format: yaml
  label: SimilarWeb Traffic and Engagement API
  slug: similarweb-traffic-and-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-traffic-and-engagement-api-openapi.yml
- filename: similarweb-traffic-sources-api-openapi.yml
  format: yaml
  label: SimilarWeb Traffic Sources API
  slug: similarweb-traffic-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-traffic-sources-api-openapi.yml
- filename: similarweb-webhooks-api-openapi.yml
  format: yaml
  label: SimilarWeb Webhooks API
  slug: similarweb-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: similarweb.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: www.similarweb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 12:15:51 2026 GMT
  host: developers.similarweb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.similarweb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Similarweb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimilarWeb, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SimilarWeb
provider_slug: similarweb
slug: similarweb-domain-security
source_filename: similarweb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.similarweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\n- host: developers.similarweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:15:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.similarweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: similarweb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/security/similarweb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Intelligence
- Web Analytics
- Traffic Analytics
- Competitive Intelligence
- Keyword Analytics
- Audience Demographics
- App Intelligence
- Market Research
- E-Commerce
- SEO
---
