---
api_specs:
- filename: spyfu-account-api-api-openapi.yml
  format: yaml
  label: SpyFu Account API API
  slug: spyfu-account-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/openapi/spyfu-account-api-api-openapi.yml
- filename: spyfu-ad-history-research-api-api-openapi.yml
  format: yaml
  label: SpyFu Ad History Research API API
  slug: spyfu-ad-history-research-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/openapi/spyfu-ad-history-research-api-api-openapi.yml
- filename: spyfu-competitors-api-api-openapi.yml
  format: yaml
  label: SpyFu Competitors API API
  slug: spyfu-competitors-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/openapi/spyfu-competitors-api-api-openapi.yml
- filename: spyfu-domain-stats-api-api-openapi.yml
  format: yaml
  label: SpyFu Domain Stats API API
  slug: spyfu-domain-stats-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/openapi/spyfu-domain-stats-api-api-openapi.yml
- filename: spyfu-keyword-research-api-api-openapi.yml
  format: yaml
  label: SpyFu Keyword Research API API
  slug: spyfu-keyword-research-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/openapi/spyfu-keyword-research-api-api-openapi.yml
- filename: spyfu-kombat-api-api-openapi.yml
  format: yaml
  label: SpyFu Kombat API API
  slug: spyfu-kombat-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/openapi/spyfu-kombat-api-api-openapi.yml
- filename: spyfu-ppc-research-api-api-openapi.yml
  format: yaml
  label: SpyFu PPC Research API API
  slug: spyfu-ppc-research-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/openapi/spyfu-ppc-research-api-api-openapi.yml
- filename: spyfu-ranking-history-api-api-openapi.yml
  format: yaml
  label: SpyFu Ranking History API API
  slug: spyfu-ranking-history-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/openapi/spyfu-ranking-history-api-api-openapi.yml
- filename: spyfu-seo-research-api-api-openapi.yml
  format: yaml
  label: SpyFu SEO Research API API
  slug: spyfu-seo-research-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/openapi/spyfu-seo-research-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spyfu.com
  spf: true
hosts:
- cert_expires: Dec  5 14:10:33 2026 GMT
  host: www.spyfu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 21:28:25 2026 GMT
  host: developer.spyfu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 14:10:33 2026 GMT
  host: api.spyfu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spyfu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpyFu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SpyFu
provider_slug: spyfu
slug: spyfu-domain-security
source_filename: spyfu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spyfu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 14:10:33 2026 GMT\n  hsts: false\n- host: developer.spyfu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:28:25 2026 GMT\n  hsts: null\n- host: api.spyfu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 14:10:33 2026 GMT\n  hsts: null\ndomains:\n- domain: spyfu.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spyfu/refs/heads/main/security/spyfu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SEO
- PPC
- Competitive Intelligence
- Keyword Research
- Ad History
- Backlinks
- Domain Analytics
- SERP
---
