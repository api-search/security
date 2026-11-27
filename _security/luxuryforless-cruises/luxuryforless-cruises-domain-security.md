---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: luxuryforless.cruises
  spf: true
hosts:
- cert_expires: Dec 25 16:54:08 2026 GMT
  host: luxuryforless.cruises
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LuxuryForLess.cruises Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LuxuryForLess.cruises, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LuxuryForLess.cruises
provider_slug: luxuryforless-cruises
slug: luxuryforless-cruises-domain-security
source_filename: luxuryforless-cruises-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luxuryforless.cruises\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 16:54:08 2026 GMT\n  hsts: false\ndomains:\n- domain: luxuryforless.cruises\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/luxuryforless-cruises/security/luxuryforless-cruises-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Cruises
- Pricing
- Data
- Aggregator
---
