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
  - 0 contactemail "tls-alerts@linkedin.com"
  caa_issue_restriction: false
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linkedin.com
  note: CAA records are present but carry only contactemail properties — there is no issue/issuewild restriction, so CAA is not constraining which CAs may issue for linkedin.com.
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: api.linkedin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: www.linkedin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: business.linkedin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: developer.linkedin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
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
overview: 'Domain security posture for LinkedIn Marketing API, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LinkedIn Marketing API
provider_slug: linkedin-ads
slug: linkedin-ads-domain-security
source_filename: linkedin-ads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  The mechanical probe only reached learn.microsoft.com (the documentation host\n  named in apis.yml). The LinkedIn hosts that actually matter — the API host and\n  the developer/member hosts — were probed by hand on the same day and are\n  recorded below with the same fields.\nhosts:\n  - host: api.linkedin.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Nov 13 23:59:59 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n  - host: www.linkedin.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep 19 23:59:59 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n  - host: business.linkedin.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep 19 23:59:59 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n  - host: developer.linkedin.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep 19 23:59:59\
  \ 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n  - host: learn.microsoft.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Dec 11 02:26:09 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\ndomains:\n  - domain: linkedin.com\n    dnssec: false\n    caa:\n      - 0 contactemail \"caarecordaware@microsoft.com\"\n      - 0 contactemail \"tls-alerts@linkedin.com\"\n    caa_issue_restriction: false\n    spf: true\n    dmarc: true\n    dmarc_policy: reject\n    note: >-\n      CAA records are present but carry only contactemail properties — there is\n      no issue/issuewild restriction, so CAA is not constraining which CAs may\n      issue for linkedin.com.\n  - domain: microsoft.com\n    dnssec: false\n    caa:\n      - 0 contactemail \"caarecordaware@microsoft.com\"\n    spf: true\n    dmarc: true\n    dmarc_policy: reject\nx-evidence:\n  fetched: '2026-08-13'\n  method_detail: openssl s_client per host, curl -I for HSTS, dig for DNSKEY/CAA/TXT/_dmarc\n"
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
