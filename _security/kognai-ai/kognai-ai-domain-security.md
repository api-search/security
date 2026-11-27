---
api_specs:
- filename: kognai-ai-golden-kog-api-openapi.yml
  format: yaml
  label: Kognai Golden Kog API
  slug: kognai-ai-golden-kog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kognai-ai/openapi/kognai-ai-golden-kog-api-openapi.yml
- filename: kognai-ai-kreativ-api-openapi.yml
  format: yaml
  label: Kognai Kreativ API
  slug: kognai-ai-kreativ-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kognai-ai/openapi/kognai-ai-kreativ-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kognai.ai
  spf: true
hosts:
- cert_expires: Jan 30 03:09:36 2027 GMT
  host: kognai.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kognai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kognai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kognai
provider_slug: kognai-ai
slug: kognai-ai-domain-security
source_filename: kognai-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kognai.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 03:09:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kognai.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kognai-ai/security/kognai-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Sovereign
- Platform
- Open Source
- Community
---
