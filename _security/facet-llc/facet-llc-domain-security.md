---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: facet.llc
  spf: true
hosts:
- cert_expires: Jan 31 04:33:59 2027 GMT
  host: facet.llc
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Facet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Facet
provider_slug: facet-llc
slug: facet-llc-domain-security
source_filename: facet-llc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: facet.llc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 04:33:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: facet.llc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/facet-llc/security/facet-llc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Payments
- Artificial Intelligence
- Agentic Commerce
- Marketplace
---
