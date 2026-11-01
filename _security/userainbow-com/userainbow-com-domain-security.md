---
api_specs:
- filename: userainbow-com-agency-api-openapi.yml
  format: yaml
  label: Rainbow Agency API
  slug: userainbow-com-agency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userainbow-com/openapi/userainbow-com-agency-api-openapi.yml
- filename: userainbow-com-appetite-api-openapi.yml
  format: yaml
  label: Rainbow Appetite API
  slug: userainbow-com-appetite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userainbow-com/openapi/userainbow-com-appetite-api-openapi.yml
- filename: userainbow-com-indication-api-openapi.yml
  format: yaml
  label: Rainbow Indication API
  slug: userainbow-com-indication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userainbow-com/openapi/userainbow-com-indication-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: userainbow.com
  spf: true
hosts:
- cert_expires: Dec 12 20:18:39 2026 GMT
  host: userainbow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Userainbow Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rainbow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rainbow
provider_slug: userainbow-com
slug: userainbow-com-domain-security
source_filename: userainbow-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userainbow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 20:18:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: userainbow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/userainbow-com/security/userainbow-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Restaurants
- Commercial Real Estate
- Beauty & Wellness
- Agents
- MGA
---
