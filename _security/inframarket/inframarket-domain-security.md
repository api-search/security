---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infra.market
  spf: true
hosts:
- cert_expires: Sep 22 12:42:15 2026 GMT
  host: www.infra.market
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inframarket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infra.Market, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Infra.Market
provider_slug: inframarket
slug: inframarket-domain-security
source_filename: inframarket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infra.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:42:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infra.market\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inframarket/refs/heads/main/security/inframarket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Construction
- Building Materials
- Manufacturing
- Marketplace
- B2B
- India
---
