---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chiquita.com
  spf: true
hosts:
- cert_expires: Sep  7 17:14:51 2026 GMT
  host: www.chiquita.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chiquita Brands International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chiquita Brands International, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chiquita Brands International
provider_slug: chiquita-brands-international
slug: chiquita-brands-international-domain-security
source_filename: chiquita-brands-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chiquita.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 17:14:51 2026 GMT\n  hsts: false\ndomains:\n- domain: chiquita.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chiquita-brands-international/refs/heads/main/security/chiquita-brands-international-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agribusiness
- Bananas
- Consumer Packaged Goods
- Distribution
- Fresh Produce
- Fruit
- Global Supply Chain
- Latin America
- Plantations
- Plantains
- Pineapples
- Retail
- Sustainability
---
