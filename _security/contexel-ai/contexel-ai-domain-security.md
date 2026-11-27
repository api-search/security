---
api_specs:
- filename: contexel-ai-openapi-generated.yml
  format: yaml
  label: Contexel API
  slug: contexel-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contexel-ai/openapi/_ae-authored/contexel-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild ";"
  - 0 iodef "mailto:security@contexel.ai"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: contexel.ai
  spf: true
hosts:
- cert_expires: Apr 12 23:59:59 2027 GMT
  host: contexel.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contexel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contexel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Contexel
provider_slug: contexel-ai
slug: contexel-ai-domain-security
source_filename: contexel-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contexel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: contexel.ai\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:security@contexel.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/contexel-ai/security/contexel-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Memory
- Family workspace
- Personal workspace
- ChatGPT
- Claude
- Cursor
---
