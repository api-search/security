---
api_specs:
- filename: bitflyer-account-api-openapi.yml
  format: yaml
  label: bitFlyer Account API
  slug: bitflyer-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-account-api-openapi.yml
- filename: bitflyer-assets-api-openapi.yml
  format: yaml
  label: bitFlyer Assets API
  slug: bitflyer-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-assets-api-openapi.yml
- filename: bitflyer-chat-api-openapi.yml
  format: yaml
  label: bitFlyer Chat API
  slug: bitflyer-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-chat-api-openapi.yml
- filename: bitflyer-deposits-and-withdrawals-api-openapi.yml
  format: yaml
  label: bitFlyer Deposits and Withdrawals API
  slug: bitflyer-deposits-and-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-deposits-and-withdrawals-api-openapi.yml
- filename: bitflyer-markets-api-openapi.yml
  format: yaml
  label: bitFlyer Markets API
  slug: bitflyer-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-markets-api-openapi.yml
- filename: bitflyer-trading-api-openapi.yml
  format: yaml
  label: bitFlyer Trading API
  slug: bitflyer-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/openapi/bitflyer-trading-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bitflyer.com
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: bitflyer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bitflyer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bitFlyer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: bitFlyer
provider_slug: bitflyer
slug: bitflyer-domain-security
source_filename: bitflyer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitflyer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bitflyer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitflyer/refs/heads/main/security/bitflyer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Japan
---
