---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tpp.network
  spf: true
hosts:
- cert_expires: Dec 31 00:22:59 2026 GMT
  host: tpp.network
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tpp Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TPP GROUP INC., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TPP GROUP INC.
provider_slug: tpp-network
slug: tpp-network-domain-security
source_filename: tpp-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tpp.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 00:22:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tpp.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tpp-network/security/tpp-network-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Media
- Intelligence
- Arabic
- Marketing
---
