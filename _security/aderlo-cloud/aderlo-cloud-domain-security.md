---
api_specs:
- filename: aderlo-cloud-api-openapi.json
  format: json
  label: Aderlo Cloud public API API
  slug: aderlo-cloud-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aderlo-cloud/openapi/_original/aderlo-cloud-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aderlo.cloud
  spf: true
hosts:
- cert_expires: Dec 23 14:18:11 2026 GMT
  host: aderlo.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aderlo Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aderlo Cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Aderlo Cloud
provider_slug: aderlo-cloud
slug: aderlo-cloud-domain-security
source_filename: aderlo-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aderlo.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 14:18:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aderlo.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/aderlo-cloud/security/aderlo-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Hosting
- WooCommerce
- WordPress
- EU
- Managed
- Cloud
---
