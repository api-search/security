---
api_specs:
- filename: fashn-openapi.yml
  format: yaml
  label: FASHN
  slug: fashn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fashn/refs/heads/main/openapi/fashn-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fashn.ai
  spf: true
hosts:
- cert_expires: Aug 20 22:33:57 2026 GMT
  host: fashn.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 22:33:57 2026 GMT
  host: api.fashn.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fashn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FASHN AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: FASHN AI
provider_slug: fashn
slug: fashn-domain-security
source_filename: fashn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fashn.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:33:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fashn.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:33:57 2026 GMT\n  hsts: null\ndomains:\n- domain: fashn.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fashn/refs/heads/main/security/fashn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Clothing
- Fashion
- Virtual Try-On
---
