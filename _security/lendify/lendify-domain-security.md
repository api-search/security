---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lendify.com
  spf: true
hosts:
- cert_expires: Dec 16 01:35:30 2026 GMT
  host: lendify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lendify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lendify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lendify
provider_slug: lendify
slug: lendify-domain-security
source_filename: lendify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lendify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 01:35:30 2026 GMT\n  hsts: false\ndomains:\n- domain: lendify.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendify/refs/heads/main/security/lendify-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Finance
- B2B
- Factoring
- Loans
- Sweden
---
