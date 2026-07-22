---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: turingsaas.com
  spf: true
hosts:
- cert_expires: Oct  1 06:46:01 2026 GMT
  host: www.turingsaas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turing Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Turing Labs
provider_slug: turing
slug: turing-domain-security
source_filename: turing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.turingsaas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:46:01 2026 GMT\n  hsts: false\ndomains:\n- domain: turingsaas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turing/refs/heads/main/security/turing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Manufacturing
- Consumer Packaged Goods
- Product Development
- Formulation
- Product-Led Growth
- SaaS
- R&D
---
