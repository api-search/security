---
api_specs:
- filename: faa-airport-status-web-service-openapi.yml
  format: yaml
  label: FAA Airport Status Web Service (ASWS)
  slug: faa-airport-status-web-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faa/refs/heads/main/openapi/faa-airport-status-web-service-openapi.yml
- filename: faa-aeronautic-product-release-api-openapi.yml
  format: yaml
  label: FAA Aeronautic Product Release API (APRA)
  slug: faa-aeronautic-product-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faa/refs/heads/main/openapi/faa-aeronautic-product-release-api-openapi.yml
- filename: faa-air-carrier-prd-api-openapi.yml
  format: yaml
  label: FAA Air Carrier PRD API
  slug: faa-air-carrier-prd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faa/refs/heads/main/openapi/faa-air-carrier-prd-api-openapi.yml
- filename: faa-safety-assurance-system-api-openapi.yml
  format: yaml
  label: FAA Safety Assurance System (SAS) API
  slug: faa-safety-assurance-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faa/refs/heads/main/openapi/faa-safety-assurance-system-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 128 issue "digicert.com"
  - 128 issue "amazon.com"
  - 128 iodef "mailto:9-ait-arin-abuse@faa.gov"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: faa.gov
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.faa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: registry.faa.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: portal.swim.faa.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Faa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Aviation Administration, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Federal Aviation Administration
provider_slug: faa
slug: faa-domain-security
source_filename: faa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.faa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: registry.faa.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\n- host: portal.swim.faa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: faa.gov\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 128 issue \"digicert.com\"\n  - 128 issue \"amazon.com\"\n  - 128 iodef \"mailto:9-ait-arin-abuse@faa.gov\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faa/refs/heads/main/security/faa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- United States
- Aviation
- Airports
- Government
- Regulator
- Open Data
- Airspace
- Drones
- Aeronautical Information
---
