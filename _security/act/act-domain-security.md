---
api_specs:
- filename: v1
  format: yaml
  label: Act! Web API
  slug: web-api
  spec_type: OpenAPI
  url: https://apimta.act.com/act.web.api/swagger/docs/v1
- filename: act-activityseries-api-openapi.yml
  format: yaml
  label: Act! CRM Activity Series API
  slug: act-activityseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-activityseries-api-openapi.yml
- filename: act-customentities-api-openapi.yml
  format: yaml
  label: Act! CRM Custom Entities API
  slug: act-customentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-customentities-api-openapi.yml
- filename: act-documenttypes-api-openapi.yml
  format: yaml
  label: Act! CRM Document Types API
  slug: act-documenttypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-documenttypes-api-openapi.yml
- filename: act-historytypes-api-openapi.yml
  format: yaml
  label: Act! CRM History Types API
  slug: act-historytypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-historytypes-api-openapi.yml
- filename: act-marketingautomations-api-openapi.yml
  format: yaml
  label: Act! CRM Marketing Automations API
  slug: act-marketingautomations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-marketingautomations-api-openapi.yml
- filename: act-metadatainfo-api-openapi.yml
  format: yaml
  label: Act! CRM Metadata Info API
  slug: act-metadatainfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-metadatainfo-api-openapi.yml
- filename: act-secondarycontacts-api-openapi.yml
  format: yaml
  label: Act! CRM Secondary Contacts API
  slug: act-secondarycontacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-secondarycontacts-api-openapi.yml
- filename: act-supplementalfiles-api-openapi.yml
  format: yaml
  label: Act! CRM Supplemental Files API
  slug: act-supplementalfiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-supplementalfiles-api-openapi.yml
- filename: act-syncdata-api-openapi.yml
  format: yaml
  label: Act! CRM Sync Data API
  slug: act-syncdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-syncdata-api-openapi.yml
- filename: act-tasktypes-api-openapi.yml
  format: yaml
  label: Act! CRM Task Types API
  slug: act-tasktypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/openapi/act-tasktypes-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "networksolutions.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: act.com
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: www.act.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: developer.act.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: apimta.act.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Act Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Act! CRM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Act! CRM
provider_slug: act
slug: act-domain-security
source_filename: act-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.act.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\n- host: developer.act.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\n- host: apimta.act.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: act.com\n  dnssec: false\n  caa:\n  - 0 issue \"networksolutions.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/act/refs/heads/main/security/act-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Customer Relationship Management
- Marketing Automation
- Contact Management
- Sales
- Opportunity Management
- OData
- Small Business
---
