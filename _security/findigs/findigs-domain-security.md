---
api_specs:
- filename: findigs-applications-api-openapi.yml
  format: yaml
  label: Findigs Applications API
  slug: findigs-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findigs/refs/heads/main/openapi/findigs-applications-api-openapi.yml
- filename: findigs-groups-api-openapi.yml
  format: yaml
  label: Findigs Groups API
  slug: findigs-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findigs/refs/heads/main/openapi/findigs-groups-api-openapi.yml
- filename: findigs-listings-api-openapi.yml
  format: yaml
  label: Findigs Listings API
  slug: findigs-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findigs/refs/heads/main/openapi/findigs-listings-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:security@findigs.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: findigs.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: getfindigs.com
  spf: false
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: www.findigs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 19:22:36 2026 GMT
  host: docs.getfindigs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.client.findigs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Findigs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Findigs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Findigs
provider_slug: findigs
slug: findigs-domain-security
source_filename: findigs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.findigs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.getfindigs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 19:22:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.client.findigs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: findigs.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:security@findigs.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getfindigs.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/findigs/refs/heads/main/security/findigs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- rental-screening
- tenant-screening
- resident-screening
- rental-application
- underwriting
- decisioning
- Identity Verification
- income-verification
- credit-check
- background-check
- fraud-detection
- property-management
- real-estate
- proptech
- fcra
- fair-housing
- Webhook
---
