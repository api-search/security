---
api_specs:
- filename: poloniex-asyncapi.yml
  format: yaml
  label: Poloniex
  slug: poloniex
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/poloniex/refs/heads/main/asyncapi/poloniex-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: poloniex.com
  spf: true
hosts:
- cert_expires: Sep 17 03:55:55 2026 GMT
  host: docs.poloniex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Poloniex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Poloniex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Poloniex
provider_slug: poloniex
slug: poloniex-domain-security
source_filename: poloniex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.poloniex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:55:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: poloniex.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poloniex/refs/heads/main/security/poloniex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Public APIs
---
