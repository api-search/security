---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sailo.com
  spf: true
hosts:
- cert_expires: Aug 21 21:03:27 2026 GMT
  host: sailo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sailo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sailo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Sailo
provider_slug: sailo
slug: sailo-domain-security
source_filename: sailo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sailo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 21:03:27 2026 GMT\n  hsts: null\ndomains:\n- domain: sailo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sailo/refs/heads/main/security/sailo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Boat Rental
- Yacht Charter
- Marketplace
- Travel
- Peer to Peer
- Boating
- Techstars
---
