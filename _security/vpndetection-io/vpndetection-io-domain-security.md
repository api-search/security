---
api_specs:
- filename: vpndetection-io-account-api-openapi.yml
  format: yaml
  label: VPNDetection Account API
  slug: vpndetection-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-account-api-openapi.yml
- filename: vpndetection-io-api-keys-api-openapi.yml
  format: yaml
  label: VPNDetection API keys API
  slug: vpndetection-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-api-keys-api-openapi.yml
- filename: vpndetection-io-authorization-api-openapi.yml
  format: yaml
  label: VPNDetection Authorization API
  slug: vpndetection-io-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-authorization-api-openapi.yml
- filename: vpndetection-io-database-api-openapi.yml
  format: yaml
  label: VPNDetection Database API
  slug: vpndetection-io-database-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-database-api-openapi.yml
- filename: vpndetection-io-entitlement-api-openapi.yml
  format: yaml
  label: VPNDetection Entitlement API
  slug: vpndetection-io-entitlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-entitlement-api-openapi.yml
- filename: vpndetection-io-lookup-api-openapi.yml
  format: yaml
  label: VPNDetection Lookup API
  slug: vpndetection-io-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-lookup-api-openapi.yml
- filename: vpndetection-io-organization-api-openapi.yml
  format: yaml
  label: VPNDetection Organization API
  slug: vpndetection-io-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vpndetection-io/openapi/vpndetection-io-organization-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vpndetection.io
  spf: true
hosts:
- cert_expires: Feb  6 14:09:22 2027 GMT
  host: vpndetection.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: VPNDetection Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VPNDetection, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VPNDetection
provider_slug: vpndetection-io
slug: vpndetection-io-domain-security
source_filename: vpndetection-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vpndetection.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 14:09:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vpndetection.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/vpndetection-io/security/vpndetection-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- VPN
- IP
- Security
- Data
- Detection
---
