---
api_specs:
- filename: companies-house-charges-api-openapi.yml
  format: yaml
  label: Companies House Charges API
  slug: companies-house-charges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-charges-api-openapi.yml
- filename: companies-house-companyprofile-api-openapi.yml
  format: yaml
  label: Companies House Company Profile API
  slug: companies-house-companyprofile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-companyprofile-api-openapi.yml
- filename: companies-house-documentlocation-api-openapi.yml
  format: yaml
  label: Companies House Document Location API
  slug: companies-house-documentlocation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-documentlocation-api-openapi.yml
- filename: companies-house-documentmetadata-api-openapi.yml
  format: yaml
  label: Companies House Document Metadata API
  slug: companies-house-documentmetadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-documentmetadata-api-openapi.yml
- filename: companies-house-exemptions-api-openapi.yml
  format: yaml
  label: Companies House Exemptions API
  slug: companies-house-exemptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-exemptions-api-openapi.yml
- filename: companies-house-filinghistory-api-openapi.yml
  format: yaml
  label: Companies House Filing History API
  slug: companies-house-filinghistory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-filinghistory-api-openapi.yml
- filename: companies-house-insolvency-api-openapi.yml
  format: yaml
  label: Companies House Insolvency API
  slug: companies-house-insolvency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-insolvency-api-openapi.yml
- filename: companies-house-officerappointments-api-openapi.yml
  format: yaml
  label: Companies House Officer Appointments API
  slug: companies-house-officerappointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-officerappointments-api-openapi.yml
- filename: companies-house-officerdisqualifications-api-openapi.yml
  format: yaml
  label: Companies House Officer Disqualifications API
  slug: companies-house-officerdisqualifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-officerdisqualifications-api-openapi.yml
- filename: companies-house-officers-api-openapi.yml
  format: yaml
  label: Companies House Officers API
  slug: companies-house-officers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-officers-api-openapi.yml
- filename: companies-house-personswithsignificantcontrol-api-openapi.yml
  format: yaml
  label: Companies House Persons With Significant Control API
  slug: companies-house-personswithsignificantcontrol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-personswithsignificantcontrol-api-openapi.yml
- filename: companies-house-personswithsignificantcontrolnotifications-api-openapi.yml
  format: yaml
  label: Companies House Persons With Significant Control Notifications API
  slug: companies-house-personswithsignificantcontrolnotifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-personswithsignificantcontrolnotifications-api-openapi.yml
- filename: companies-house-registeredofficeaddress-api-openapi.yml
  format: yaml
  label: Companies House Registered Office Address API
  slug: companies-house-registeredofficeaddress-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-registeredofficeaddress-api-openapi.yml
- filename: companies-house-registers-api-openapi.yml
  format: yaml
  label: Companies House Registers API
  slug: companies-house-registers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-registers-api-openapi.yml
- filename: companies-house-search-api-openapi.yml
  format: yaml
  label: Companies House Search API
  slug: companies-house-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-search-api-openapi.yml
- filename: companies-house-ukestablishments-api-openapi.yml
  format: yaml
  label: Companies House UK Establishments API
  slug: companies-house-ukestablishments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companies-house/openapi/companies-house-ukestablishments-api-openapi.yml
description: ''
domains:
- caa:
  - www-cdn.production.govuk.service.gov.uk.
  - www-gov-uk.map.fastly.net.
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: true
  domain: www.gov.uk
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: service.gov.uk
  spf: true
hosts:
- cert_expires: Dec 28 22:06:14 2026 GMT
  host: www.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  4 23:59:59 2027 GMT
  host: developer-specs.company-information.service.gov.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  4 23:59:59 2027 GMT
  host: stream.companieshouse.gov.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Companies House Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Companies House, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Companies House
provider_slug: companies-house
slug: companies-house-domain-security
source_filename: companies-house-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 22:06:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer-specs.company-information.service.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 23:59:59 2027 GMT\n  hsts: null\n- host: stream.companieshouse.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: www.gov.uk\n  dnssec: true\n  caa:\n  - www-cdn.production.govuk.service.gov.uk.\n  - www-gov-uk.map.fastly.net.\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n- domain: service.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/companies-house/security/companies-house-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Companies
- UK Government
- Business Registration
- Company Search
- Officers
- Filing History
- Insolvency
- Charges
- Persons of Significant Control
- Open Data
---
