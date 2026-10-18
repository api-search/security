---
api_specs:
- filename: actava-models-api-openapi.yml
  format: yaml
  label: Actava.ai Models API
  slug: actava-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actava/refs/heads/main/openapi/actava-models-api-openapi.yml
- filename: actava-chat-completions-api-openapi.yml
  format: yaml
  label: Actava.ai Chat Completions API
  slug: actava-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actava/refs/heads/main/openapi/actava-chat-completions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:operations@actava.ai"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: actava.ai
  spf: true
hosts:
- cert_expires: Nov 21 21:56:39 2026 GMT
  host: actava.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Actava Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actava.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Actava.ai
provider_slug: actava
slug: actava-domain-security
source_filename: actava-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: actava.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 21:56:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: actava.ai\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:operations@actava.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actava/refs/heads/main/security/actava-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Healthcare
- Machine Learning
- Platform
---
