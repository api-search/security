---
api_specs:
- filename: sam-gov-location-services-openapi.yml
  format: yaml
  label: SAM.gov Public Location Services API
  slug: location-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sam.gov/refs/heads/main/openapi/sam-gov-location-services-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sam.gov
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "entrust.net"
  - 0 issue "godaddy.com"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gsa.gov
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: sam.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 10:21:32 2026 GMT
  host: open.gsa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.sam.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sam.Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAM.gov, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAM.gov
provider_slug: sam.gov
slug: sam.gov-domain-security
source_filename: sam.gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sam.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open.gsa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sam.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sam.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gsa.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sam.gov/refs/heads/main/security/sam.gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Procurement
- Contracts
- Entity Management
- Location Services
- GSA
---
