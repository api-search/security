---
api_specs:
- filename: agl-energy-data-holder-customers-api-openapi.yml
  format: yaml
  label: AGL Energy Data Holder Customers API
  slug: agl-energy-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-data-holder-customers-api-openapi.yml
- filename: agl-energy-data-holder-operations-api-openapi.yml
  format: yaml
  label: AGL Energy Data Holder Operations API
  slug: agl-energy-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-data-holder-operations-api-openapi.yml
- filename: agl-energy-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: AGL Energy Distributed Energy Resources API
  slug: agl-energy-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-distributed-energy-resources-api-openapi.yml
- filename: agl-energy-electricity-service-points-api-openapi.yml
  format: yaml
  label: AGL Energy Electricity Service Points API
  slug: agl-energy-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-electricity-service-points-api-openapi.yml
- filename: agl-energy-electricity-usage-api-openapi.yml
  format: yaml
  label: AGL Energy Electricity Usage API
  slug: agl-energy-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-electricity-usage-api-openapi.yml
- filename: agl-energy-energy-account-balances-api-openapi.yml
  format: yaml
  label: AGL Energy Energy Account Balances API
  slug: agl-energy-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-account-balances-api-openapi.yml
- filename: agl-energy-energy-account-billing-api-openapi.yml
  format: yaml
  label: AGL Energy Energy Account Billing API
  slug: agl-energy-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-account-billing-api-openapi.yml
- filename: agl-energy-energy-accounts-api-openapi.yml
  format: yaml
  label: AGL Energy Energy Accounts API
  slug: agl-energy-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-accounts-api-openapi.yml
- filename: agl-energy-energy-plans-api-openapi.yml
  format: yaml
  label: AGL Energy Energy Plans API
  slug: agl-energy-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-plans-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agl.com.au
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energymadeeasy.gov.au
  spf: true
  spf_record: v=spf1 include:amazonses.com -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aer.gov.au
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: www.agl.com.au
  hsts: true
  hsts_header: max-age=86400 ; includeSubDomains ; preload
  hsts_max_age: 86400
  hsts_note: max-age is 1 day — well below the 31536000 (1 year) that HSTS preload submission requires, despite the preload token being present.
  http_status: 403
  http_status_note: Akamai edge (server AkamaiGHost) denies all non-browser clients.
  https: true
  role: corporate website
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: public.cdr.agl.com.au
  hsts: true
  hsts_header: max-age=63072000; includeSubDomains;
  hsts_max_age: 63072000
  http_status: 200
  http_status_note: 200 on /cds-au/v1/discovery/status; nginx 404 at the host root, which is correct.
  https: true
  other_headers:
  - 'x-content-type-options: nosniff'
  - 'x-frame-options: DENY'
  - 'access-control-allow-origin: *'
  role: AGL CDR public base URI
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: cdr.energymadeeasy.gov.au
  hsts: false
  hsts_note: No Strict-Transport-Security header returned on the AGL PRD path.
  http_status: 200
  https: true
  operated_by: Australian Energy Regulator (not AGL)
  role: AER-operated central energy Product Reference Data host serving AGL's plans
  tls_version: TLSv1.3
- cert_expires: Oct  5 08:19:20 2026 GMT
  host: www.aer.gov.au
  hsts: null
  https: true
  role: AER documentation host referenced from apis.yml
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agl Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AGL Energy, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AGL Energy
provider_slug: agl-energy
slug: agl-energy-domain-security
source_filename: agl-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\n  (0-working/probe-domain-security.py), corrected and extended by hand on the\n  same date: the script's HSTS check reported null for hosts that do serve\n  Strict-Transport-Security, and it did not cover the AER-operated Product\n  Reference Data host that serves AGL's plans. Both were re-probed with\n  `curl -D -` and `dig`, and the observed header values are recorded verbatim.\nhosts:\n- host: www.agl.com.au\n  role: corporate website\n  https: true\n  http_status: 403\n  http_status_note: Akamai edge (server AkamaiGHost) denies all non-browser clients.\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_header: 'max-age=86400 ; includeSubDomains ; preload'\n  hsts_max_age: 86400\n  hsts_note: >-\n    max-age is 1 day — well below the 31536000 (1 year) that HSTS preload\n    submission requires, despite the preload token being present.\n\
  - host: public.cdr.agl.com.au\n  role: AGL CDR public base URI\n  https: true\n  http_status: 200\n  http_status_note: 200 on /cds-au/v1/discovery/status; nginx 404 at the host root, which is correct.\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_header: 'max-age=63072000; includeSubDomains;'\n  hsts_max_age: 63072000\n  other_headers:\n  - 'x-content-type-options: nosniff'\n  - 'x-frame-options: DENY'\n  - 'access-control-allow-origin: *'\n- host: cdr.energymadeeasy.gov.au\n  role: AER-operated central energy Product Reference Data host serving AGL's plans\n  operated_by: Australian Energy Regulator (not AGL)\n  https: true\n  http_status: 200\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: false\n  hsts_note: No Strict-Transport-Security header returned on the AGL PRD path.\n- host: www.aer.gov.au\n  role: AER documentation host referenced from apis.yml\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5\
  \ 08:19:20 2026 GMT\n  hsts: null\ndomains:\n- domain: agl.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: energymadeeasy.gov.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  spf_record: 'v=spf1 include:amazonses.com -all'\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aer.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nsummary:\n  hosts_probed: 4\n  https_everywhere: true\n  tls_1_3_everywhere: true\n  hsts_on_api_host: true\n  dnssec_anywhere: false\n  caa_published: [agl.com.au, energymadeeasy.gov.au]\n  dmarc_enforcing: [agl.com.au (reject), aer.gov.au (reject), energymadeeasy.gov.au\
  \ (quarantine)]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/security/agl-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retailer
- Consumer Data Right
- CDR
- Smart Metering
- Solar
- DER
- Renewables
- Energy Markets
---
