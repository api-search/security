---
api_specs:
- filename: okx-asyncapi.yml
  format: yaml
  label: OKEx
  slug: okex
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/okex/refs/heads/main/asyncapi/okx-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: okex.com
  spf: false
hosts:
- host: www.okex.com
  https: false
kind: domain-security
layout: security
method: probed
name: Okex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OKEx, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: OKEx
provider_slug: okex
slug: okex-domain-security
source_filename: okex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.okex.com\n  https: false\ndomains:\n- domain: okex.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okex/refs/heads/main/security/okex-domain-security.yml
summary_line: DNSSEC
tags:
- Cryptocurrency
- Public APIs
---
