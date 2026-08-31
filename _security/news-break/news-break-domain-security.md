---
api_specs:
- filename: news-break-account-billing-api-openapi.yml
  format: yaml
  label: News Break Account Billing API
  slug: news-break-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-account-billing-api-openapi.yml
- filename: news-break-ad-account-api-openapi.yml
  format: yaml
  label: News Break Ad Account API
  slug: news-break-ad-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-ad-account-api-openapi.yml
- filename: news-break-ad-api-openapi.yml
  format: yaml
  label: News Break Ad API
  slug: news-break-ad-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-ad-api-openapi.yml
- filename: news-break-ad-set-api-openapi.yml
  format: yaml
  label: News Break Ad Set API
  slug: news-break-ad-set-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-ad-set-api-openapi.yml
- filename: news-break-campaign-api-openapi.yml
  format: yaml
  label: News Break Campaign API
  slug: news-break-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-campaign-api-openapi.yml
- filename: news-break-event-management-api-openapi.yml
  format: yaml
  label: News Break Event Management API
  slug: news-break-event-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-event-management-api-openapi.yml
- filename: news-break-organization-api-openapi.yml
  format: yaml
  label: News Break Organization API
  slug: news-break-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-organization-api-openapi.yml
- filename: news-break-report-api-openapi.yml
  format: yaml
  label: News Break Report API
  slug: news-break-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-report-api-openapi.yml
- filename: news-break-reporting-api-openapi.yml
  format: yaml
  label: News Break Reporting API
  slug: news-break-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/openapi/news-break-reporting-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: newsbreak.com
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.newsbreak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:43:59 2026 GMT
  host: advertising-api.newsbreak.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: business.newsbreak.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 15 12:54:26 2026 GMT
  host: msp-platform.newsbreak.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 12:56:36 2026 GMT
  host: doc.msp.newsbreak.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: News Break Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for News Break, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: News Break
provider_slug: news-break
slug: news-break-domain-security
source_filename: news-break-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newsbreak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: advertising-api.newsbreak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:43:59 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: business.newsbreak.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\n- host: msp-platform.newsbreak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:54:26 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n- host: doc.msp.newsbreak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:56:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\nfindings:\n- severity: notable\n  host: business.newsbreak.com\n  finding:\
  \ >-\n    The Advertising API host - the one that carries the Access-Token bearer credential on every\n    request - negotiates only TLSv1.2 and serves NO Strict-Transport-Security header, while every\n    other NewsBreak host in scope is TLSv1.3 with HSTS. It is the weakest transport posture on the\n    estate and it is the host handling the secrets.\n- severity: notable\n  domain: newsbreak.com\n  finding: >-\n    No CAA record and no DNSSEC. Any CA can issue for newsbreak.com and its subdomains, and DNS\n    answers are unauthenticated.\n- severity: minor\n  domain: newsbreak.com\n  finding: DMARC policy is p=quarantine rather than p=reject.\n- severity: minor\n  host: advertising-api.newsbreak.com\n  finding: >-\n    HSTS max-age is 259200 (3 days), below the 31536000 (1 year) preload threshold, and does not\n    set includeSubDomains.\ndomains:\n- domain: newsbreak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/news-break/refs/heads/main/security/news-break-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- News
- Media
- Local News
- Publishing
- Monetization
- Campaign Management
- Reporting
- Analytics
- Content
---
