---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: graphiterx.com
  spf: true
hosts:
- cert_expires: Dec 24 22:19:10 2026 GMT
  host: www.graphiterx.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Graphiterx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GraphiteRx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GraphiteRx
provider_slug: graphiterx
slug: graphiterx-domain-security
source_filename: graphiterx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.graphiterx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 22:19:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: graphiterx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/graphiterx/security/graphiterx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare Commerce
- Pharmacy Procurement
- 340B Compliance
- Pharma E‑commerce
- B2B Marketplace
- AI Technology
---
