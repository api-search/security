---
api_specs:
- filename: getclarity-ai-media-statement-api-openapi.yml
  format: yaml
  label: Clarity Media Statement API
  slug: getclarity-ai-media-statement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclarity-ai/openapi/getclarity-ai-media-statement-api-openapi.yml
- filename: getclarity-ai-users-api-openapi.yml
  format: yaml
  label: Clarity Users API
  slug: getclarity-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclarity-ai/openapi/getclarity-ai-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getclarity.ai
  spf: true
hosts:
- cert_expires: Dec 13 06:10:24 2026 GMT
  host: www.getclarity.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getclarity Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clarity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Clarity
provider_slug: getclarity-ai
slug: getclarity-ai-domain-security
source_filename: getclarity-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getclarity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 06:10:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getclarity.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getclarity-ai/security/getclarity-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Hiring fraud
- Identity verification
- Deepfake detection
- Talent acquisition security
- AI hiring security
---
