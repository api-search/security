---
api_specs:
- filename: nearbypermits-com-address-api-openapi.yml
  format: yaml
  label: Nearby Permits Address API
  slug: nearbypermits-com-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nearbypermits-com/openapi/nearbypermits-com-address-api-openapi.yml
- filename: nearbypermits-com-cities-api-openapi.yml
  format: yaml
  label: Nearby Permits Cities API
  slug: nearbypermits-com-cities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nearbypermits-com/openapi/nearbypermits-com-cities-api-openapi.yml
- filename: nearbypermits-com-near-api-openapi.yml
  format: yaml
  label: Nearby Permits Near API
  slug: nearbypermits-com-near-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nearbypermits-com/openapi/nearbypermits-com-near-api-openapi.yml
- filename: nearbypermits-com-permit-api-openapi.yml
  format: yaml
  label: Nearby Permits Permit API
  slug: nearbypermits-com-permit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nearbypermits-com/openapi/nearbypermits-com-permit-api-openapi.yml
- filename: nearbypermits-com-recent-api-openapi.yml
  format: yaml
  label: Nearby Permits Recent API
  slug: nearbypermits-com-recent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nearbypermits-com/openapi/nearbypermits-com-recent-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nearbypermits.com
  spf: true
hosts:
- cert_expires: Feb  2 01:14:58 2027 GMT
  host: nearbypermits.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nearby Permits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nearby Permits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nearby Permits
provider_slug: nearbypermits-com
slug: nearbypermits-com-domain-security
source_filename: nearbypermits-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nearbypermits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 01:14:58 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nearbypermits.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nearbypermits-com/security/nearbypermits-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Permits
- Construction
---
