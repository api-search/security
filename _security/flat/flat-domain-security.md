---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clau.com
  spf: true
hosts:
- cert_expires: Aug 16 20:01:42 2026 GMT
  host: clau.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flat
provider_slug: flat
slug: flat-domain-security
source_filename: flat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clau.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:01:42 2026 GMT\n  hsts: false\ndomains:\n- domain: clau.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flat/refs/heads/main/security/flat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Proptech
- Fintech
- Mortgages
- Marketplace
- Mexico
---
