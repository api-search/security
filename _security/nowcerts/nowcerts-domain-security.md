---
api_specs:
- filename: nowcerts-openapi.yml
  format: yaml
  label: NowCerts Insureds API
  slug: nowcerts-insureds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-openapi.yml
- filename: nowcerts-openapi.yml
  format: yaml
  label: NowCerts Policies API
  slug: nowcerts-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-openapi.yml
- filename: nowcerts-openapi.yml
  format: yaml
  label: NowCerts Carriers API
  slug: nowcerts-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-openapi.yml
- filename: nowcerts-openapi.yml
  format: yaml
  label: NowCerts Endorsements API
  slug: nowcerts-endorsements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-openapi.yml
- filename: nowcerts-openapi.yml
  format: yaml
  label: NowCerts Tasks API
  slug: nowcerts-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nowcerts.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.nowcerts.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.nowcerts.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nowcerts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NowCerts, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NowCerts
provider_slug: nowcerts
slug: nowcerts-domain-security
source_filename: nowcerts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nowcerts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.nowcerts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: nowcerts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/security/nowcerts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Agency Management System
- AMS
- Policies
- Insureds
- Certificates of Insurance
- REST
---
