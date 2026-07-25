---
api_specs:
- filename: linkedin-ads-adaccounts-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdAccounts API
  slug: linkedin-ads-adaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adaccounts-api-openapi.yml
- filename: linkedin-ads-adbudgetpricing-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdBudgetPricing API
  slug: linkedin-ads-adbudgetpricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adbudgetpricing-api-openapi.yml
- filename: linkedin-ads-adtargetingentities-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdTargetingEntities API
  slug: linkedin-ads-adtargetingentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adtargetingentities-api-openapi.yml
- filename: linkedin-ads-adtargetingfacets-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AdTargetingFacets API
  slug: linkedin-ads-adtargetingfacets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-adtargetingfacets-api-openapi.yml
- filename: linkedin-ads-audiencecounts-api-openapi.yml
  format: yaml
  label: LinkedIn Marketing API AudienceCounts API
  slug: linkedin-ads-audiencecounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/openapi/linkedin-ads-audiencecounts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linkedin Ads Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinkedIn Marketing API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LinkedIn Marketing API
provider_slug: linkedin-ads
slug: linkedin-ads-domain-security
source_filename: linkedin-ads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkedin-ads/refs/heads/main/security/linkedin-ads-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Marketing
- LinkedIn
- Lead Generation
- Audience Targeting
- Conversions API
- Social Marketing
---
