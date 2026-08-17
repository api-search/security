---
api_specs:
- filename: yoast-pages-api-openapi.yml
  format: yaml
  label: Yoast Pages API
  slug: yoast-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-pages-api-openapi.yml
- filename: yoast-posts-api-openapi.yml
  format: yaml
  label: Yoast Posts API
  slug: yoast-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-posts-api-openapi.yml
- filename: yoast-seo-head-api-openapi.yml
  format: yaml
  label: Yoast SEO Head API
  slug: yoast-seo-head-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-seo-head-api-openapi.yml
- filename: yoast-abilities-api-openapi.yml
  format: yaml
  label: Yoast SEO Abilities API
  slug: yoast-abilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-abilities-api-openapi.yml
- filename: yoast-schema-aggregator-openapi.yml
  format: yaml
  label: Yoast Schema Aggregator API
  slug: yoast-schema-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-schema-aggregator-openapi.yml
- filename: yoast-myyoast-provisioning-openapi.yml
  format: yaml
  label: MyYoast Provisioning API
  slug: myyoast-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-myyoast-provisioning-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: yoast.com
  spf: true
hosts:
- cert_expires: Sep 18 14:43:29 2026 GMT
  host: yoast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 01:47:04 2026 GMT
  host: developer.yoast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 05:19:35 2026 GMT
  host: my.yoast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yoast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yoast, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Yoast
provider_slug: yoast
slug: yoast-domain-security
source_filename: yoast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yoast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:43:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.yoast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:47:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.yoast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 05:19:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yoast.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/security/yoast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SEO
- WordPress
- Content Optimization
- Schema
- Metadata
- Structured Data
- Headless CMS
- Content Analysis
- Agent Readiness
- Plugins
---
