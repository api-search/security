---
api_specs:
- filename: adt-access-codes-api-openapi.yml
  format: yaml
  label: ADT Access Codes API
  slug: adt-access-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-access-codes-api-openapi.yml
- filename: adt-access-control-api-openapi.yml
  format: yaml
  label: ADT Access Control API
  slug: adt-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-access-control-api-openapi.yml
- filename: adt-automation-api-openapi.yml
  format: yaml
  label: ADT Automation API
  slug: adt-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-automation-api-openapi.yml
- filename: adt-devices-api-openapi.yml
  format: yaml
  label: ADT Devices API
  slug: adt-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-devices-api-openapi.yml
- filename: adt-events-api-openapi.yml
  format: yaml
  label: ADT Events API
  slug: adt-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-events-api-openapi.yml
- filename: adt-reports-api-openapi.yml
  format: yaml
  label: ADT Reports API
  slug: adt-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-reports-api-openapi.yml
- filename: adt-security-systems-api-openapi.yml
  format: yaml
  label: ADT Security Systems API
  slug: adt-security-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-security-systems-api-openapi.yml
- filename: adt-sites-api-openapi.yml
  format: yaml
  label: ADT Sites API
  slug: adt-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-sites-api-openapi.yml
- filename: adt-users-api-openapi.yml
  format: yaml
  label: ADT Users API
  slug: adt-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-users-api-openapi.yml
- filename: adt-video-api-openapi.yml
  format: yaml
  label: ADT Video API
  slug: adt-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-video-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adt.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.adt.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'Read from the response headers of an HTTP/2 403 (www.adt.com''s Akamai edge denies every automated client, including /robots.txt). The header is served: "strict-transport-security: max-age=31536000 ; includeSubDomains". probe-domain-security.py recorded null on 2026-08-30 because it only reads HSTS off a 2xx; corrected by hand.'
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.adt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADT, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ADT
provider_slug: adt
slug: adt-domain-security
source_filename: adt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    Read from the response headers of an HTTP/2 403 (www.adt.com's Akamai edge denies every\n    automated client, including /robots.txt). The header is served:\n    \"strict-transport-security: max-age=31536000 ; includeSubDomains\". probe-domain-security.py\n    recorded null on 2026-08-30 because it only reads HSTS off a 2xx; corrected by hand.\n- host: api.adt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: adt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/security/adt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
- Fortune 1000
---
