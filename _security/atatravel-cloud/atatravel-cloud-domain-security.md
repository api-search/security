---
api_specs:
- filename: atatravel-cloud-buildings-api-openapi.yml
  format: yaml
  label: ATA Travel Buildings API
  slug: atatravel-cloud-buildings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atatravel-cloud/openapi/atatravel-cloud-buildings-api-openapi.yml
- filename: atatravel-cloud-commercial-api-openapi.yml
  format: yaml
  label: ATA Travel Commercial API
  slug: atatravel-cloud-commercial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atatravel-cloud/openapi/atatravel-cloud-commercial-api-openapi.yml
- filename: atatravel-cloud-discovery-api-openapi.yml
  format: yaml
  label: ATA Travel Discovery API
  slug: atatravel-cloud-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atatravel-cloud/openapi/atatravel-cloud-discovery-api-openapi.yml
- filename: atatravel-cloud-properties-api-openapi.yml
  format: yaml
  label: ATA Travel Properties API
  slug: atatravel-cloud-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/atatravel-cloud/openapi/atatravel-cloud-properties-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atatravel.cloud
  spf: true
hosts:
- cert_expires: Dec 17 12:44:46 2026 GMT
  host: atatravel.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 21:06:13 2026 GMT
  host: api.atatravel.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: ATA Travel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ATA Travel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ATA Travel
provider_slug: atatravel-cloud
slug: atatravel-cloud-domain-security
source_filename: atatravel-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atatravel.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 12:44:46 2026 GMT\n  hsts: false\n- host: api.atatravel.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 21:06:13 2026 GMT\n  hsts: null\ndomains:\n- domain: atatravel.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/atatravel-cloud/security/atatravel-cloud-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Artificial Intelligence
- Booking
- Accommodation
- Software-as-a-Service
- NoCommission
---
