---
api_specs:
- filename: kucoin-asyncapi.yml
  format: yaml
  label: KuCoin
  slug: kucoin
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/kucoin/main/asyncapi/kucoin-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kucoin.com
  spf: true
hosts:
- cert_expires: Oct  7 04:44:13 2026 GMT
  host: docs.kucoin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kucoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KuCoin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KuCoin
provider_slug: kucoin
slug: kucoin-domain-security
source_filename: kucoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.kucoin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:44:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kucoin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kucoin/refs/heads/main/security/kucoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Public APIs
---
