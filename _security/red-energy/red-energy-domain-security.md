---
api_specs:
- filename: red-energy-data-holder-customers-api-openapi.yml
  format: yaml
  label: Red Energy Data Holder Customers API
  slug: red-energy-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-data-holder-customers-api-openapi.yml
- filename: red-energy-data-holder-operations-api-openapi.yml
  format: yaml
  label: Red Energy Data Holder Operations API
  slug: red-energy-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-data-holder-operations-api-openapi.yml
- filename: red-energy-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Red Energy Distributed Energy Resources API
  slug: red-energy-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-distributed-energy-resources-api-openapi.yml
- filename: red-energy-electricity-service-points-api-openapi.yml
  format: yaml
  label: Red Energy Electricity Service Points API
  slug: red-energy-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-electricity-service-points-api-openapi.yml
- filename: red-energy-electricity-usage-api-openapi.yml
  format: yaml
  label: Red Energy Electricity Usage API
  slug: red-energy-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-electricity-usage-api-openapi.yml
- filename: red-energy-energy-account-balances-api-openapi.yml
  format: yaml
  label: Red Energy Energy Account Balances API
  slug: red-energy-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-account-balances-api-openapi.yml
- filename: red-energy-energy-account-billing-api-openapi.yml
  format: yaml
  label: Red Energy Energy Account Billing API
  slug: red-energy-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-account-billing-api-openapi.yml
- filename: red-energy-energy-accounts-api-openapi.yml
  format: yaml
  label: Red Energy Energy Accounts API
  slug: red-energy-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-accounts-api-openapi.yml
- filename: red-energy-energy-plans-api-openapi.yml
  format: yaml
  label: Red Energy Energy Plans API
  slug: red-energy-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-plans-api-openapi.yml
description: ''
domains:
- caa: []
  caa_note: No CAA record published — any public CA may issue for this domain.
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: redenergy.com.au
  spf: true
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energymadeeasy.gov.au
  note: Australian Energy Regulator host, not a Red Energy domain.
  spf: true
hosts:
- cert_expires: Oct 12 03:45:46 2026 GMT
  host: www.redenergy.com.au
  hsts: null
  hsts_note: Undetermined. Every request returns HTTP 403 with a Cloudflare bot challenge, so no response from the origin was observed. Absence of the header on the challenge page is not evidence about the site.
  http_status: 403
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: cdr.energymadeeasy.gov.au
  hsts: false
  hsts_note: Confirmed absent. GET /red-energy/cds-au/v1/energy/plans returned HTTP 200 with no strict-transport-security header. Fronted by Amazon CloudFront and API Gateway.
  http_status: 200
  https: true
  security_headers:
    access-control-allow-origin: '*'
    access-control-expose-headers: x-v, Retry-After, x-fapi-interaction-id
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: public.cdr.redenergy.com.au
  hsts: true
  hsts_corrected: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_note: Corrected from the script's null. GET /cds-au/v1/discovery/status returned strict-transport-security "max-age=63072000; includeSubDomains;" on 2026-07-27. The script probed the host root, which returns an nginx 404 with no security headers.
  http_status: 200
  https: true
  security_headers:
    access-control-allow-headers: Range,x-v,x-min-v
    access-control-allow-origin: '*'
    access-control-expose-headers: Content-Length,x-v,x-min-v
    strict-transport-security: max-age=63072000; includeSubDomains;
    x-content-type-options: nosniff
    x-frame-options: DENY
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Red Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Red Energy
provider_slug: red-energy
slug: red-energy-domain-security
source_filename: red-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of the apis.yml and OpenAPI servers[] hosts, run by\n  0-working/probe-domain-security.py, then corrected by hand for HSTS: the\n  script's HEAD-based check returned null on all three hosts, but a GET against\n  a path each host actually serves showed public.cdr.redenergy.com.au does send\n  Strict-Transport-Security. Corrections are marked.\nhosts:\n- host: www.redenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:45:46 2026 GMT\n  hsts: null\n  hsts_note: >-\n    Undetermined. Every request returns HTTP 403 with a Cloudflare bot challenge,\n    so no response from the origin was observed. Absence of the header on the\n    challenge page is not evidence about the site.\n  http_status: 403\n- host: cdr.energymadeeasy.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: false\n  hsts_note: >-\n    Confirmed absent. GET /red-energy/cds-au/v1/energy/plans\
  \ returned HTTP 200\n    with no strict-transport-security header. Fronted by Amazon CloudFront and\n    API Gateway.\n  http_status: 200\n  security_headers:\n    access-control-allow-origin: '*'\n    access-control-expose-headers: x-v, Retry-After, x-fapi-interaction-id\n- host: public.cdr.redenergy.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_corrected: true\n  hsts_note: >-\n    Corrected from the script's null. GET /cds-au/v1/discovery/status returned\n    strict-transport-security \"max-age=63072000; includeSubDomains;\" on\n    2026-07-27. The script probed the host root, which returns an nginx 404 with\n    no security headers.\n  http_status: 200\n  security_headers:\n    strict-transport-security: max-age=63072000; includeSubDomains;\n    x-content-type-options: nosniff\n    x-frame-options: DENY\n    access-control-allow-origin: '*'\n    access-control-allow-headers:\
  \ Range,x-v,x-min-v\n    access-control-expose-headers: Content-Length,x-v,x-min-v\ndomains:\n- domain: redenergy.com.au\n  dnssec: true\n  caa: []\n  caa_note: No CAA record published — any public CA may issue for this domain.\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: energymadeeasy.gov.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  note: Australian Energy Regulator host, not a Red Energy domain.\nfindings:\n  strong:\n    - DNSSEC signed on redenergy.com.au.\n    - DMARC at p=reject on redenergy.com.au — the strictest policy.\n    - TLS 1.3 on all three hosts.\n    - Two-year HSTS with includeSubDomains on the CDR public base URI.\n  gaps:\n    - No CAA record on redenergy.com.au.\n    - No security.txt on any host (see well-known/red-energy-well-known.yml).\n    - No vulnerability disclosure\
  \ programme or trust centre found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/security/red-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Product Reference Data
- Smart Metering
- Open Data
---
