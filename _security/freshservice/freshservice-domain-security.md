---
api_specs:
- filename: freshservice-agents-api-openapi.yml
  format: yaml
  label: Freshservice Agents API
  slug: freshservice-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/openapi/freshservice-agents-api-openapi.yml
- filename: freshservice-assets-api-openapi.yml
  format: yaml
  label: Freshservice Assets API
  slug: freshservice-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/openapi/freshservice-assets-api-openapi.yml
- filename: freshservice-changes-api-openapi.yml
  format: yaml
  label: Freshservice Changes API
  slug: freshservice-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/openapi/freshservice-changes-api-openapi.yml
- filename: freshservice-groups-api-openapi.yml
  format: yaml
  label: Freshservice Groups API
  slug: freshservice-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/openapi/freshservice-groups-api-openapi.yml
- filename: freshservice-problems-api-openapi.yml
  format: yaml
  label: Freshservice Problems API
  slug: freshservice-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/openapi/freshservice-problems-api-openapi.yml
- filename: freshservice-releases-api-openapi.yml
  format: yaml
  label: Freshservice Releases API
  slug: freshservice-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/openapi/freshservice-releases-api-openapi.yml
- filename: freshservice-requesters-api-openapi.yml
  format: yaml
  label: Freshservice Requesters API
  slug: freshservice-requesters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/openapi/freshservice-requesters-api-openapi.yml
- filename: freshservice-tickets-api-openapi.yml
  format: yaml
  label: Freshservice Tickets API
  slug: freshservice-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/openapi/freshservice-tickets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freshworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freshservice.com
  spf: true
hosts:
- cert_expires: Aug 22 10:30:03 2026 GMT
  host: www.freshworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.freshservice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: <domain>.freshservice.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''<domain>.fr'
kind: domain-security
layout: security
method: probed
name: Freshservice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freshservice, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Freshservice
provider_slug: freshservice
slug: freshservice-domain-security
source_filename: freshservice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freshworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:30:03 2026 GMT\n  hsts: null\n- host: api.freshservice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: <domain>.freshservice.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''<domain>.fr'\n  hsts: null\ndomains:\n- domain: freshworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: freshservice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshservice/refs/heads/main/security/freshservice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ITSM
- Help Desk
- Ticketing
- Asset Management
- Change Management
- Freshworks
---
