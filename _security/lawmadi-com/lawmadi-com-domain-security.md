---
api_specs:
- filename: lawmadi-com-agent-discovery-api-openapi.yml
  format: yaml
  label: Lawmadi Agent discovery API
  slug: lawmadi-com-agent-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-agent-discovery-api-openapi.yml
- filename: lawmadi-com-ask-api-openapi.yml
  format: yaml
  label: Lawmadi Ask API
  slug: lawmadi-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-ask-api-openapi.yml
- filename: lawmadi-com-ask-stream-api-openapi.yml
  format: yaml
  label: Lawmadi Ask Stream API
  slug: lawmadi-com-ask-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-ask-stream-api-openapi.yml
- filename: lawmadi-com-pricing-api-openapi.yml
  format: yaml
  label: Lawmadi Pricing API
  slug: lawmadi-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-pricing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lawmadi.com
  spf: true
hosts:
- cert_expires: Feb  9 06:39:32 2027 GMT
  host: lawmadi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lawmadi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lawmadi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lawmadi
provider_slug: lawmadi-com
slug: lawmadi-com-domain-security
source_filename: lawmadi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lawmadi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 06:39:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lawmadi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lawmadi-com/security/lawmadi-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- Artificial Intelligence
- Korean
- Law
---
