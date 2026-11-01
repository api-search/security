---
api_specs:
- filename: flyreel-conversation-api-openapi.yml
  format: yaml
  label: Flyreel Conversation API
  slug: flyreel-conversation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyreel/openapi/flyreel-conversation-api-openapi.yml
- filename: flyreel-inspection-api-openapi.yml
  format: yaml
  label: Flyreel Inspection API
  slug: flyreel-inspection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyreel/openapi/flyreel-inspection-api-openapi.yml
- filename: flyreel-webhook-api-openapi.yml
  format: yaml
  label: Flyreel Webhook API
  slug: flyreel-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyreel/openapi/flyreel-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flyreel.co
  spf: true
hosts:
- cert_expires: Dec 26 20:36:25 2026 GMT
  host: www.flyreel.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flyreel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flyreel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flyreel
provider_slug: flyreel
slug: flyreel-domain-security
source_filename: flyreel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flyreel.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 20:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flyreel.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flyreel/security/flyreel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Risk
- API
- Data
- Analytics
---
