---
api_specs:
- filename: connells-branches-api-openapi.yml
  format: yaml
  label: Connells Group Branches API
  slug: connells-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connells/refs/heads/main/openapi/connells-branches-api-openapi.yml
- filename: connells-locations-api-openapi.yml
  format: yaml
  label: Connells Group Locations API
  slug: connells-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connells/refs/heads/main/openapi/connells-locations-api-openapi.yml
- filename: connells-people-api-openapi.yml
  format: yaml
  label: Connells Group People API
  slug: connells-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connells/refs/heads/main/openapi/connells-people-api-openapi.yml
- filename: connells-testimonials-api-openapi.yml
  format: yaml
  label: Connells Group Testimonials API
  slug: connells-testimonials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connells/refs/heads/main/openapi/connells-testimonials-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: connellsgroup.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: connells.co.uk
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.connellsgroup.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 07:14:58 2026 GMT
  host: www.connells.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.countrywide.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Connells Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connells Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Connells Group
provider_slug: connells
slug: connells-domain-security
source_filename: connells-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.connellsgroup.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: www.connells.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 07:14:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.countrywide.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: connellsgroup.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: connells.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connells/refs/heads/main/security/connells-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- Property Listings
- Brokerage
- Estate Agency
- Rentals
- Valuation
- Conveyancing
- Mortgage
- Property Management
- Auctions
- PropTech
---
