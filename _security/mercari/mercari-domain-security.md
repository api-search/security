---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mercari.com
  spf: true
hosts:
- cert_expires: Aug 25 10:41:53 2026 GMT
  host: www.mercari.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 17:53:33 2026 GMT
  host: about.mercari.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercari, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mercari
provider_slug: mercari
slug: mercari-domain-security
source_filename: mercari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mercari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:41:53 2026 GMT\n  hsts: null\n- host: about.mercari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 17:53:33 2026 GMT\n  hsts: false\ndomains:\n- domain: mercari.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercari/refs/heads/main/security/mercari-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketplace
- Resale
- P2P
- Ecommerce
---
