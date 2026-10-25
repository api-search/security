---
api_specs:
- filename: icao-geo-api-openapi.yml
  format: yaml
  label: ICAO GEO API
  slug: icao-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-geo-api-openapi.yml
- filename: icao-icao-api-openapi.yml
  format: yaml
  label: ICAO ICAO API
  slug: icao-icao-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-icao-api-openapi.yml
- filename: icao-infomation-api-openapi.yml
  format: yaml
  label: ICAO Infomation API
  slug: icao-infomation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-infomation-api-openapi.yml
- filename: icao-publication-api-openapi.yml
  format: yaml
  label: ICAO Publication API
  slug: icao-publication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-publication-api-openapi.yml
- filename: icao-safety-api-openapi.yml
  format: yaml
  label: ICAO Safety API
  slug: icao-safety-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-safety-api-openapi.yml
- filename: icao-usoap-api-openapi.yml
  format: yaml
  label: ICAO USOAP API
  slug: icao-usoap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/openapi/icao-usoap-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: icao.int
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.icao.int
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: applications.icao.int
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Icao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ICAO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ICAO
provider_slug: icao
slug: icao-domain-security
source_filename: icao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icao.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: applications.icao.int\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: icao.int\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/security/icao-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Airlines
- Airports
- Airspace
- Aviation
- Reference Data
- Standards
- United Nations
---
