---
api_specs:
- filename: energy-queensland-data-holder-customers-api-openapi.yml
  format: yaml
  label: Energy Queensland Data Holder Customers API
  slug: energy-queensland-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-data-holder-customers-api-openapi.yml
- filename: energy-queensland-data-holder-operations-api-openapi.yml
  format: yaml
  label: Energy Queensland Data Holder Operations API
  slug: energy-queensland-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-data-holder-operations-api-openapi.yml
- filename: energy-queensland-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Energy Queensland Distributed Energy Resources API
  slug: energy-queensland-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-distributed-energy-resources-api-openapi.yml
- filename: energy-queensland-electricity-service-points-api-openapi.yml
  format: yaml
  label: Energy Queensland Electricity Service Points API
  slug: energy-queensland-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-electricity-service-points-api-openapi.yml
- filename: energy-queensland-electricity-usage-api-openapi.yml
  format: yaml
  label: Energy Queensland Electricity Usage API
  slug: energy-queensland-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-electricity-usage-api-openapi.yml
- filename: energy-queensland-energy-account-balances-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Account Balances API
  slug: energy-queensland-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-account-balances-api-openapi.yml
- filename: energy-queensland-energy-account-billing-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Account Billing API
  slug: energy-queensland-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-account-billing-api-openapi.yml
- filename: energy-queensland-energy-accounts-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Accounts API
  slug: energy-queensland-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-accounts-api-openapi.yml
- filename: energy-queensland-energy-plans-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Plans API
  slug: energy-queensland-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-plans-api-openapi.yml
description: Transport and DNS security posture across the Energy Queensland estate. Two things stand out. First, the CDR host is the best-configured surface the group operates - HSTS with a two-year max-age and includeSubDomains, nosniff, and DENY framing - which is unsurprising given it was built to a mandated security profile rather than by choice. Second, every domain in the group shares one mail security configuration (SPF pointing at spf.energyq.com.au and Mimecast, DMARC p=reject with the same reporting mailbox), a clear signature of the 2016 Ergon/Energex merger into a single ICT function. No Energy Queensland domain has DNSSEC, and none publishes CAA records.
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: energyq.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ergonretail.com.au
  note: The registrable domain behind both public.cdr and api.cdr - i.e. the entire CDR estate.
  spf: true
  spf_record: v=spf1 include:spf.energyq.com.au include:au._netblocks.mimecast.com -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ergon.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: energex.com.au
  spf: true
  spf_record: v=spf1 include:spf.energyq.com.au include:au._netblocks.mimecast.com include:amazonses.com -all
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energymadeeasy.gov.au
  note: Australian Energy Regulator domain, not Energy Queensland's. The only domain in scope with CAA records.
  spf: true
hosts:
- cert_expires: Sep 24 01:59:30 2026 GMT
  host: www.energyq.com.au
  hsts: null
  https: true
  note: Behind a Cloudflare managed challenge - returns HTTP 403 to every programmatic client, so response headers cannot be observed.
  role: Energy Queensland group website
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: cdr.energymadeeasy.gov.au
  hsts: false
  https: true
  note: AWS API Gateway behind CloudFront. No HSTS header on a live 200 response.
  observed_headers:
    access-control-allow-origin: '*'
    access-control-expose-headers: x-v, Retry-After, x-fapi-interaction-id
  role: AER Energy Made Easy CDR host serving Ergon-branded Product Reference Data (not an Energy Queensland host)
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: public.cdr.ergonretail.com.au
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  note: Observed on a live HTTP 200 from /cds-au/v1/discovery/status on 2026-07-27. The automated probe recorded hsts null because the site root 404s; the header is present on real endpoints.
  observed_headers:
    access-control-allow-headers: Range, x-v, x-min-v
    access-control-allow-origin: '*'
    access-control-max-age: '3600'
    strict-transport-security: max-age=63072000; includeSubDomains;
    x-content-type-options: nosniff
    x-frame-options: DENY
  role: Ergon Energy Retail registered CDR public base URI
  tls_version: TLSv1.3
- host: api.cdr.ergonretail.com.au
  https: true
  mtls_required: true
  note: The TLS handshake emits "Request CERT (13)" with a private CDR certificate chain - the server demands a client certificate issued by the CDR Register certificate authority. No HTTP response is obtainable without one, so no response headers are recorded.
  role: Ergon Energy Retail CDR consumer-data resource host
- host: auth.cdr.ergonretail.com.au
  https: true
  note: Serves HTTP but returns 404 at the root, at /.well-known/oauth-authorization-server and at /cds-au/v1/discovery/status. Recorded for what it returned; NOT assumed to be the InfoSec base URI.
  role: resolves in DNS; purpose unconfirmed
kind: domain-security
layout: security
method: probed
name: Energy Queensland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Energy Queensland, probed live across 5 host(s) and 5 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Energy Queensland
provider_slug: energy-queensland
slug: energy-queensland-domain-security
source_filename: energy-queensland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of the apis.yml and OpenAPI hosts via\n  0-working/probe-domain-security.py, extended with the three registrable\n  domains the automated pass did not reach (ergonretail.com.au, ergon.com.au,\n  energex.com.au) and with HSTS observed on a real 200 response rather than on a\n  HEAD to a 404 path.\ndescription: >-\n  Transport and DNS security posture across the Energy Queensland estate. Two\n  things stand out. First, the CDR host is the best-configured surface the group\n  operates - HSTS with a two-year max-age and includeSubDomains, nosniff, and\n  DENY framing - which is unsurprising given it was built to a mandated security\n  profile rather than by choice. Second, every domain in the group shares one\n  mail security configuration (SPF pointing at spf.energyq.com.au and Mimecast,\n  DMARC p=reject with the same reporting mailbox), a clear signature of the 2016\n  Ergon/Energex merger into a\
  \ single ICT function. No Energy Queensland domain\n  has DNSSEC, and none publishes CAA records.\nhosts:\n  - host: www.energyq.com.au\n    role: Energy Queensland group website\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep 24 01:59:30 2026 GMT\n    hsts: null\n    note: >-\n      Behind a Cloudflare managed challenge - returns HTTP 403 to every\n      programmatic client, so response headers cannot be observed.\n  - host: cdr.energymadeeasy.gov.au\n    role: AER Energy Made Easy CDR host serving Ergon-branded Product Reference Data (not an Energy Queensland host)\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Jan 31 23:59:59 2027 GMT\n    hsts: false\n    observed_headers:\n      access-control-allow-origin: '*'\n      access-control-expose-headers: x-v, Retry-After, x-fapi-interaction-id\n    note: AWS API Gateway behind CloudFront. No HSTS header on a live 200 response.\n  - host: public.cdr.ergonretail.com.au\n    role: Ergon Energy Retail registered\
  \ CDR public base URI\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Oct 18 23:59:59 2026 GMT\n    hsts: true\n    hsts_max_age: 63072000\n    hsts_include_subdomains: true\n    observed_headers:\n      strict-transport-security: max-age=63072000; includeSubDomains;\n      x-content-type-options: nosniff\n      x-frame-options: DENY\n      access-control-allow-origin: '*'\n      access-control-allow-headers: Range, x-v, x-min-v\n      access-control-max-age: '3600'\n    note: >-\n      Observed on a live HTTP 200 from /cds-au/v1/discovery/status on\n      2026-07-27. The automated probe recorded hsts null because the site root\n      404s; the header is present on real endpoints.\n  - host: api.cdr.ergonretail.com.au\n    role: Ergon Energy Retail CDR consumer-data resource host\n    https: true\n    mtls_required: true\n    note: >-\n      The TLS handshake emits \"Request CERT (13)\" with a private CDR certificate\n      chain - the server demands a client certificate\
  \ issued by the CDR Register\n      certificate authority. No HTTP response is obtainable without one, so no\n      response headers are recorded.\n  - host: auth.cdr.ergonretail.com.au\n    role: resolves in DNS; purpose unconfirmed\n    https: true\n    note: >-\n      Serves HTTP but returns 404 at the root, at\n      /.well-known/oauth-authorization-server and at /cds-au/v1/discovery/status.\n      Recorded for what it returned; NOT assumed to be the InfoSec base URI.\ndomains:\n  - domain: energyq.com.au\n    dnssec: false\n    caa: []\n    spf: true\n    dmarc: true\n    dmarc_policy: reject\n  - domain: ergonretail.com.au\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: v=spf1 include:spf.energyq.com.au include:au._netblocks.mimecast.com -all\n    dmarc: true\n    dmarc_policy: reject\n    note: The registrable domain behind both public.cdr and api.cdr - i.e. the entire CDR estate.\n  - domain: ergon.com.au\n    dnssec: false\n    caa: []\n    spf: true\n    dmarc:\
  \ true\n    dmarc_policy: reject\n  - domain: energex.com.au\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: v=spf1 include:spf.energyq.com.au include:au._netblocks.mimecast.com include:amazonses.com -all\n    dmarc: true\n    dmarc_policy: reject\n  - domain: energymadeeasy.gov.au\n    dnssec: false\n    caa:\n      - 0 issuewild \"amazontrust.com\"\n      - 0 issuewild \"awstrust.com\"\n      - 0 issuewild \"amazon.com\"\n      - 0 issuewild \"amazonaws.com\"\n    spf: true\n    dmarc: true\n    dmarc_policy: quarantine\n    note: Australian Energy Regulator domain, not Energy Queensland's. The only domain in scope with CAA records.\nfindings:\n  - All four Energy Queensland domains publish SPF and a DMARC policy of p=reject with a shared reporting mailbox - a strong, consistent mail posture.\n  - No domain in the group has DNSSEC enabled.\n  - No Energy Queensland domain publishes CAA records, so certificate issuance is unconstrained.\n  - HSTS is present only on the\
  \ CDR public base URI, the one host built to a mandated security profile.\n  - The corporate sites are unobservable from outside a browser (Cloudflare 403), which also means no security.txt or disclosure policy page could be verified. See well-known/energy-queensland-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/security/energy-queensland-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Distribution Network
- Energy Retail
- Consumer Data Right
- CDR
- Product Reference Data
- Queensland
- Smart Metering
- Solar
- DER
- Open Data
---
