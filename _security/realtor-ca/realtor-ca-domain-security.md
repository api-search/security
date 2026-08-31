---
api_specs:
- filename: realtor-ca-destination-api-openapi.yml
  format: yaml
  label: REALTOR.ca Destination API
  slug: realtor-ca-destination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/openapi/realtor-ca-destination-api-openapi.yml
- filename: realtor-ca-lead-api-openapi.yml
  format: yaml
  label: REALTOR.ca Lead API
  slug: realtor-ca-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/openapi/realtor-ca-lead-api-openapi.yml
- filename: realtor-ca-member-api-openapi.yml
  format: yaml
  label: REALTOR.ca Member API
  slug: realtor-ca-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/openapi/realtor-ca-member-api-openapi.yml
- filename: realtor-ca-office-api-openapi.yml
  format: yaml
  label: REALTOR.ca Office API
  slug: realtor-ca-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/openapi/realtor-ca-office-api-openapi.yml
- filename: realtor-ca-openhouse-api-openapi.yml
  format: yaml
  label: REALTOR.ca Open House API
  slug: realtor-ca-openhouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/openapi/realtor-ca-openhouse-api-openapi.yml
- filename: realtor-ca-property-api-openapi.yml
  format: yaml
  label: REALTOR.ca Property API
  slug: realtor-ca-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/openapi/realtor-ca-property-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: realtor.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crea.ca
  spf: true
hosts:
- cert_expires: Sep 14 19:31:29 2026 GMT
  host: www.realtor.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 07:36:09 2026 GMT
  host: www.crea.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:31:29 2026 GMT
  host: ddfapi-docs.realtor.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Realtor Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REALTOR.ca, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: REALTOR.ca
provider_slug: realtor-ca
slug: realtor-ca-domain-security
source_filename: realtor-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.realtor.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:31:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.crea.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 07:36:09 2026 GMT\n  hsts: false\n- host: ddfapi-docs.realtor.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:31:29 2026 GMT\n  hsts: null\ndomains:\n- domain: realtor.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: crea.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtor-ca/refs/heads/main/security/realtor-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Canada
- Property Listings
- MLS
- RESO
- IDX
- Listing Syndication
- PropTech
- OData
- Rentals
---
