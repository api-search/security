---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: shoponpickle.com
  spf: true
hosts:
- cert_expires: Oct 11 10:51:41 2026 GMT
  host: shoponpickle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pickle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pickle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pickle
provider_slug: pickle
slug: pickle-domain-security
source_filename: pickle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shoponpickle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 10:51:41 2026 GMT\n  hsts: null\ndomains:\n- domain: shoponpickle.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pickle/refs/heads/main/security/pickle-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Marketplace
- Fashion
- Rental
- Resale
- Peer-to-Peer
- Ecommerce
- Consumer
---
