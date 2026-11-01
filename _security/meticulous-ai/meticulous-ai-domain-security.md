---
api_specs:
- filename: meticulous-ai-openapi-generated.yml
  format: yaml
  label: Meticulous Ai API
  slug: meticulous-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meticulous-ai/openapi/_ae-authored/meticulous-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meticulous.ai
  spf: true
hosts:
- cert_expires: Mar 23 23:59:59 2027 GMT
  host: www.meticulous.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meticulous Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meticulous Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meticulous Ai
provider_slug: meticulous-ai
slug: meticulous-ai-domain-security
source_filename: meticulous-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meticulous.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: meticulous.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/meticulous-ai/security/meticulous-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Testing
- Automation
- Frontend
- VisualRegression
---
