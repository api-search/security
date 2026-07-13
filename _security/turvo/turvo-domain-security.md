---
api_specs:
- filename: turvo-openapi.yml
  format: yaml
  label: Turvo Shipments API
  slug: turvo-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-openapi.yml
- filename: turvo-openapi.yml
  format: yaml
  label: Turvo Orders API
  slug: turvo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-openapi.yml
- filename: turvo-openapi.yml
  format: yaml
  label: Turvo Locations API
  slug: turvo-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-openapi.yml
- filename: turvo-openapi.yml
  format: yaml
  label: Turvo Accounts API
  slug: turvo-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-openapi.yml
- filename: turvo-openapi.yml
  format: yaml
  label: Turvo Carriers API
  slug: turvo-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-openapi.yml
- filename: turvo-openapi.yml
  format: yaml
  label: Turvo Tracking API
  slug: turvo-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/openapi/turvo-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: turvo.com
  spf: true
hosts:
- cert_expires: Sep 29 10:04:41 2026 GMT
  host: turvo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: help.turvo.com
  https: false
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: publicapi.turvo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turvo, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Turvo
provider_slug: turvo
slug: turvo-domain-security
source_filename: turvo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: turvo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:04:41 2026 GMT\n  hsts: false\n- host: help.turvo.com\n  https: false\n- host: publicapi.turvo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: turvo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turvo/refs/heads/main/security/turvo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Logistics
- Transportation Management System
- TMS
- Supply Chain
- Freight
- Shipments
- Carriers
---
