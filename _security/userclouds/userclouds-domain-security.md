---
api_specs:
- filename: userclouds-accessors-api-openapi.yml
  format: yaml
  label: UserClouds Accessors API
  slug: userclouds-accessors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userclouds/openapi/userclouds-accessors-api-openapi.yml
- filename: userclouds-columnretentiondurations-api-openapi.yml
  format: yaml
  label: UserClouds Column Retention Durations API
  slug: userclouds-columnretentiondurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userclouds/openapi/userclouds-columnretentiondurations-api-openapi.yml
- filename: userclouds-columns-api-openapi.yml
  format: yaml
  label: UserClouds Columns API
  slug: userclouds-columns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userclouds/openapi/userclouds-columns-api-openapi.yml
- filename: userclouds-data-types-api-openapi.yml
  format: yaml
  label: UserClouds Data Types API
  slug: userclouds-data-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userclouds/openapi/userclouds-data-types-api-openapi.yml
- filename: userclouds-mutators-api-openapi.yml
  format: yaml
  label: UserClouds Mutators API
  slug: userclouds-mutators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userclouds/openapi/userclouds-mutators-api-openapi.yml
- filename: userclouds-purposes-api-openapi.yml
  format: yaml
  label: UserClouds Purposes API
  slug: userclouds-purposes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userclouds/openapi/userclouds-purposes-api-openapi.yml
- filename: userclouds-user-search-indices-api-openapi.yml
  format: yaml
  label: UserClouds User Search Indices API
  slug: userclouds-user-search-indices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userclouds/openapi/userclouds-user-search-indices-api-openapi.yml
- filename: userclouds-users-api-openapi.yml
  format: yaml
  label: UserClouds Users API
  slug: userclouds-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userclouds/openapi/userclouds-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: userclouds.com
  spf: true
hosts:
- cert_expires: Jan  4 08:38:19 2027 GMT
  host: userclouds.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Userclouds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UserClouds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UserClouds
provider_slug: userclouds
slug: userclouds-domain-security
source_filename: userclouds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userclouds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 08:38:19 2027 GMT\n  hsts: false\ndomains:\n- domain: userclouds.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/userclouds/security/userclouds-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
