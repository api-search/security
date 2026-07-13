---
api_specs:
- filename: lusd_total_supply.txt
  format: yaml
  label: Liquity V1 Circulating Supply API
  slug: liquity-v1-circulating-supply-api
  spec_type: OpenAPI
  url: https://api.liquity.org/v1/lusd_total_supply.txt
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: liquity.org
  spf: false
hosts:
- cert_expires: Sep 20 13:39:19 2026 GMT
  host: api.liquity.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liquity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liquity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Liquity
provider_slug: liquity
slug: liquity-domain-security
source_filename: liquity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.liquity.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 13:39:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: liquity.org\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquity/refs/heads/main/security/liquity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Decentralized Finance
- Lending
- Stablecoin
- Ethereum
- LUSD
- BOLD
- Liquidity Protocol
---
