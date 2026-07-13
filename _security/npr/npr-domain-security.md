---
api_specs:
- filename: npr-station-finder-openapi-original.yml
  format: yaml
  label: NPR Station Finder
  slug: station-finder
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npr/main/openapi/npr-station-finder-openapi-original.yml
- filename: npr-identity-openapi-original.yml
  format: yaml
  label: NPR Identity
  slug: identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npr/main/openapi/npr-identity-openapi-original.yml
- filename: npr-authorization-openapi-original.yml
  format: yaml
  label: NPR Authorization
  slug: authorization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/npr/main/openapi/npr-authorization-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: npr.org
  spf: true
hosts:
- cert_expires: Sep 17 17:25:28 2026 GMT
  host: www.npr.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: dev.npr.org
  https: false
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: listening.api.npr.org
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Npr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NPR, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NPR
provider_slug: npr
slug: npr-domain-security
source_filename: npr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.npr.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:25:28 2026 GMT\n  hsts: false\n- host: dev.npr.org\n  https: false\n- host: listening.api.npr.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: npr.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/npr/refs/heads/main/security/npr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Media
- News
- Radio
---
