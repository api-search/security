---
api_specs:
- filename: federal-highway-administration-authentication-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Authentication API
  slug: federal-highway-administration-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-authentication-api-openapi.yml
- filename: federal-highway-administration-configuration-rest-controller-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Configuration Rest Controller API
  slug: federal-highway-administration-configuration-rest-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-configuration-rest-controller-api-openapi.yml
- filename: federal-highway-administration-deposit-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Deposit API
  slug: federal-highway-administration-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-deposit-api-openapi.yml
- filename: federal-highway-administration-geofence-deployments-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Geofence Deployments API
  slug: federal-highway-administration-geofence-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-geofence-deployments-api-openapi.yml
- filename: federal-highway-administration-geofence-expiration-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Geofence Expiration API
  slug: federal-highway-administration-geofence-expiration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-geofence-expiration-api-openapi.yml
- filename: federal-highway-administration-path-management-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Path Management API
  slug: federal-highway-administration-path-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-path-management-api-openapi.yml
- filename: federal-highway-administration-registration-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Registration API
  slug: federal-highway-administration-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-registration-api-openapi.yml
- filename: federal-highway-administration-secret-management-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Secret Management API
  slug: federal-highway-administration-secret-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-secret-management-api-openapi.yml
- filename: federal-highway-administration-tim-configuration-api-openapi.yml
  format: yaml
  label: Federal Highway Administration TIM Configuration API
  slug: federal-highway-administration-tim-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-tim-configuration-api-openapi.yml
- filename: federal-highway-administration-user-limits-management-api-openapi.yml
  format: yaml
  label: Federal Highway Administration User Limits Management API
  slug: federal-highway-administration-user-limits-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-user-limits-management-api-openapi.yml
- filename: federal-highway-administration-vendor-limits-management-api-openapi.yml
  format: yaml
  label: Federal Highway Administration Vendor Limits Management API
  slug: federal-highway-administration-vendor-limits-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/openapi/federal-highway-administration-vendor-limits-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dot.gov
  spf: false
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: highways.dot.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Federal Highway Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Highway Administration, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Federal Highway Administration
provider_slug: federal-highway-administration
slug: federal-highway-administration-domain-security
source_filename: federal-highway-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highways.dot.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dot.gov\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-highway-administration/refs/heads/main/security/federal-highway-administration-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal-Government
- Transportation
- Highways
- Bridge
- Connected Vehicles
- V2X
- Open-Source
- Open Data
---
