---
api_specs:
- filename: simply-energy-data-holder-customers-api-openapi.yml
  format: yaml
  label: Simply Energy Data Holder Customers API
  slug: simply-energy-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-data-holder-customers-api-openapi.yml
- filename: simply-energy-data-holder-operations-api-openapi.yml
  format: yaml
  label: Simply Energy Data Holder Operations API
  slug: simply-energy-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-data-holder-operations-api-openapi.yml
- filename: simply-energy-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Simply Energy Distributed Energy Resources API
  slug: simply-energy-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-distributed-energy-resources-api-openapi.yml
- filename: simply-energy-electricity-service-points-api-openapi.yml
  format: yaml
  label: Simply Energy Electricity Service Points API
  slug: simply-energy-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-electricity-service-points-api-openapi.yml
- filename: simply-energy-electricity-usage-api-openapi.yml
  format: yaml
  label: Simply Energy Electricity Usage API
  slug: simply-energy-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-electricity-usage-api-openapi.yml
- filename: simply-energy-energy-account-balances-api-openapi.yml
  format: yaml
  label: Simply Energy Energy Account Balances API
  slug: simply-energy-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-energy-account-balances-api-openapi.yml
- filename: simply-energy-energy-account-billing-api-openapi.yml
  format: yaml
  label: Simply Energy Energy Account Billing API
  slug: simply-energy-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-energy-account-billing-api-openapi.yml
- filename: simply-energy-energy-accounts-api-openapi.yml
  format: yaml
  label: Simply Energy Energy Accounts API
  slug: simply-energy-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-energy-accounts-api-openapi.yml
- filename: simply-energy-energy-plans-api-openapi.yml
  format: yaml
  label: Simply Energy Energy Plans API
  slug: simply-energy-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-energy-plans-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: simplyenergy.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: engie.com.au
  spf: true
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energymadeeasy.gov.au
  probed: '2026-07-27'
  role: Australian Energy Regulator host serving CDR generic tariff data on this retailer's behalf - not owned or operated by the retailer
  spf: true
  spf_record: v=spf1 include:amazonses.com -all
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: public.cdr.engie.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  probed: '2026-07-27'
  role: registered CDR Public Base URI (apis[].baseURL) - added manually, the automated probe reads only apis.yml Website/Portal/humanURL hosts
  security_headers:
    x-content-type-options: nosniff
    x-frame-options: DENY
  tls_issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M01
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: www.simplyenergy.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: engie.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: cdr.energymadeeasy.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simply Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simply Energy, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Simply Energy
provider_slug: simply-energy
slug: simply-energy-domain-security
source_filename: simply-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: public.cdr.engie.com.au\n  role: registered CDR Public Base URI (apis[].baseURL) - added manually, the automated probe\n    reads only apis.yml Website/Portal/humanURL hosts\n  https: true\n  tls_version: TLSv1.3\n  tls_issuer: 'C=US, O=Amazon, CN=Amazon RSA 2048 M01'\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  security_headers:\n    x-content-type-options: nosniff\n    x-frame-options: DENY\n  probed: '2026-07-27'\n- host: www.simplyenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: null\n- host: engie.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\n- host: cdr.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\n\
  domains:\n- domain: simplyenergy.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: engie.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: energymadeeasy.gov.au\n  role: Australian Energy Regulator host serving CDR generic tariff data on this retailer's\n    behalf - not owned or operated by the retailer\n  dnssec: false\n  caa: ['0 issuewild \"amazonaws.com\"', '0 issuewild \"amazontrust.com\"', '0 issuewild \"awstrust.com\"',\n    '0 issuewild \"amazon.com\"']\n  spf: true\n  spf_record: v=spf1 include:amazonses.com -all\n  dmarc: true\n  dmarc_policy: quarantine\n  probed: '2026-07-27'\nfindings:\n- The retailer's own registered CDR Public Base URI (public.cdr.engie.com.au) is the strongest\n  host in this provider's surface - TLS 1.3, HSTS with a two-year max-age and includeSubDomains,\n  nosniff and DENY framing.\n- Neither corporate domain (simplyenergy.com.au, engie.com.au) publishes\
  \ a CAA record or\n  DNSSEC, and neither web host returned an HSTS header to the probe. Both sit behind Cloudflare\n  and return HTTP 403 to automated fetchers, so the HSTS result for those two hosts is\n  unconfirmed rather than proven absent.\n- Both corporate domains publish SPF and a DMARC policy of p=reject, which is the strongest\n  possible DMARC posture.\n- energymadeeasy.gov.au is included because it is an apis[].baseURL host, but it belongs to the\n  Australian Energy Regulator. Its posture should not be credited to or held against this\n  retailer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/security/simply-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Smart Metering
- Energy Markets
---
