---
api_specs:
- filename: hiveclaw-ai-openapi-generated.yml
  format: yaml
  label: HiveClaw API
  slug: hiveclaw-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hiveclaw-ai/openapi/_ae-authored/hiveclaw-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hiveclaw.ai
  spf: true
hosts:
- cert_expires: Jan 28 15:00:12 2027 GMT
  host: hiveclaw.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HiveClaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiveClaw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HiveClaw
provider_slug: hiveclaw-ai
slug: hiveclaw-ai-domain-security
source_filename: hiveclaw-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hiveclaw.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 15:00:12 2027 GMT\n  hsts: false\ndomains:\n- domain: hiveclaw.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hiveclaw-ai/security/hiveclaw-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
