---
api_specs:
- filename: us-dot-faa-aeronautic-product-release-api-openapi.yml
  format: yaml
  label: FAA Aeronautic Product Release API (APRA)
  slug: faa-aeronautic-product-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-aeronautic-product-release-api-openapi.yml
- filename: us-dot-faa-air-carrier-prd-api-openapi.yml
  format: yaml
  label: FAA Air Carrier Pilot Records Database (PRD) API
  slug: faa-air-carrier-prd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-air-carrier-prd-api-openapi.yml
- filename: us-dot-faa-safety-assurance-system-api-openapi.yml
  format: yaml
  label: FAA Safety Assurance System (SAS) API
  slug: faa-safety-assurance-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-safety-assurance-system-api-openapi.yml
- filename: us-dot-its-jpo-ode-rest-api-openapi.yml
  format: yaml
  label: USDOT ITS JPO Operational Data Environment (ODE) REST API
  slug: its-jpo-ode-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-its-jpo-ode-rest-api-openapi.yml
- filename: us-dot-faa-airport-status-web-service-openapi.yml
  format: yaml
  label: U.S. Department of Transportation Airport Status Web Service
  slug: us-dot-faa-airport-status-web-service-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-airport-status-web-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: transportation.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bts.gov
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.transportation.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:28:12 2026 GMT
  host: data.transportation.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 15 18:23:49 2026 GMT
  host: data.bts.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Us Dot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for U.S. Department of Transportation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: U.S. Department of Transportation
provider_slug: us-dot
slug: us-dot-domain-security
source_filename: us-dot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transportation.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\n- host: data.transportation.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 23:28:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.bts.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 18:23:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: transportation.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bts.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/security/us-dot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- United States
- Aviation
- Airlines
- Airports
- Government
- Regulator
- Distribution
- Aviation Consumer Protection
- Open Data
- Transportation
- Safety
- Statistics
- Automotive
- Rail
---
