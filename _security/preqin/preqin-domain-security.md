---
api_specs:
- filename: preqin-active-user-subscription-info-api-openapi.yml
  format: yaml
  label: Preqin Active User Subscription Info API
  slug: preqin-active-user-subscription-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-active-user-subscription-info-api-openapi.yml
- filename: preqin-connect-api-openapi.yml
  format: yaml
  label: Preqin Connect API
  slug: preqin-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-connect-api-openapi.yml
- filename: preqin-deal-api-openapi.yml
  format: yaml
  label: Preqin Deal API
  slug: preqin-deal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-deal-api-openapi.yml
- filename: preqin-fund-api-openapi.yml
  format: yaml
  label: Preqin Fund API
  slug: preqin-fund-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-fund-api-openapi.yml
- filename: preqin-fund-manager-api-openapi.yml
  format: yaml
  label: Preqin Fund Manager API
  slug: preqin-fund-manager-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-fund-manager-api-openapi.yml
- filename: preqin-fund-performance-api-openapi.yml
  format: yaml
  label: Preqin Fund Performance API
  slug: preqin-fund-performance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-fund-performance-api-openapi.yml
- filename: preqin-investment-consultant-api-openapi.yml
  format: yaml
  label: Preqin Investment Consultant API
  slug: preqin-investment-consultant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-investment-consultant-api-openapi.yml
- filename: preqin-investor-api-openapi.yml
  format: yaml
  label: Preqin Investor API
  slug: preqin-investor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-investor-api-openapi.yml
- filename: preqin-investor-commitment-add-on-api-openapi.yml
  format: yaml
  label: Preqin Investor Commitment (Add-on) API
  slug: preqin-investor-commitment-add-on-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-investor-commitment-add-on-api-openapi.yml
- filename: preqin-news-api-openapi.yml
  format: yaml
  label: Preqin News API
  slug: preqin-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-news-api-openapi.yml
- filename: preqin-service-provider-api-openapi.yml
  format: yaml
  label: Preqin Service Provider API
  slug: preqin-service-provider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/preqin/openapi/preqin-service-provider-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:infosec@preqin.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: preqin.com
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: www.preqin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Preqin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Preqin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Preqin
provider_slug: preqin
slug: preqin-domain-security
source_filename: preqin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.preqin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: preqin.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:infosec@preqin.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/preqin/security/preqin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Alternative Assets
- Data
- Analytics
- Private Markets
- Research
---
