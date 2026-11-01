---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nefeli.com
  spf: false
hosts:
- cert_expires: Dec 31 19:44:02 2026 GMT
  host: nefeli.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nefeli Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nefeli Networks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Nefeli Networks
provider_slug: nefeli-networks
slug: nefeli-networks-domain-security
source_filename: nefeli-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nefeli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 19:44:02 2026 GMT\n  hsts: null\ndomains:\n- domain: nefeli.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nefeli-networks/security/nefeli-networks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloudflare
- Networking
- Multi-cloud
- Edge
- SaaS
---
