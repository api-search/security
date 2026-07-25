---
api_specs:
- filename: western-digital-authentication-api-openapi.yml
  format: yaml
  label: western-digital Authentication API
  slug: western-digital-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-digital/refs/heads/main/openapi/western-digital-authentication-api-openapi.yml
- filename: western-digital-configuration-api-openapi.yml
  format: yaml
  label: western-digital Configuration API
  slug: western-digital-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-digital/refs/heads/main/openapi/western-digital-configuration-api-openapi.yml
- filename: western-digital-device-api-openapi.yml
  format: yaml
  label: western-digital Device API
  slug: western-digital-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-digital/refs/heads/main/openapi/western-digital-device-api-openapi.yml
- filename: western-digital-files-api-openapi.yml
  format: yaml
  label: western-digital Files API
  slug: western-digital-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-digital/refs/heads/main/openapi/western-digital-files-api-openapi.yml
- filename: western-digital-search-api-openapi.yml
  format: yaml
  label: western-digital Search API
  slug: western-digital-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-digital/refs/heads/main/openapi/western-digital-search-api-openapi.yml
- filename: western-digital-sharing-api-openapi.yml
  format: yaml
  label: western-digital Sharing API
  slug: western-digital-sharing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-digital/refs/heads/main/openapi/western-digital-sharing-api-openapi.yml
- filename: western-digital-user-api-openapi.yml
  format: yaml
  label: western-digital User API
  slug: western-digital-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-digital/refs/heads/main/openapi/western-digital-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: westerndigital.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mycloud.com
  spf: true
hosts:
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: www.westerndigital.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: developer.westerndigital.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: device.mycloud.com
  https: false
kind: domain-security
layout: security
method: probed
name: Western Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for western-digital, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: western-digital
provider_slug: western-digital
slug: western-digital-domain-security
source_filename: western-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westerndigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.westerndigital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: null\n- host: device.mycloud.com\n  https: false\ndomains:\n- domain: westerndigital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mycloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-digital/refs/heads/main/security/western-digital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
---
