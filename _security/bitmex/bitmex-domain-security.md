---
api_specs:
- filename: bitmex-asyncapi.yml
  format: yaml
  label: Bitmex
  slug: bitmex
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitmex/refs/heads/main/asyncapi/bitmex-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitmex.com
  spf: true
hosts:
- cert_expires: Sep 15 04:29:15 2026 GMT
  host: www.bitmex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitmex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitmex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bitmex
provider_slug: bitmex
slug: bitmex-domain-security
source_filename: bitmex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bitmex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:29:15 2026 GMT\n  hsts: false\ndomains:\n- domain: bitmex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitmex/refs/heads/main/security/bitmex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cryptocurrency
- Public APIs
---
