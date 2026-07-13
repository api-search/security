---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fruityvice.com
  spf: true
hosts:
- cert_expires: Aug 26 09:39:58 2026 GMT
  host: www.fruityvice.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fruityvice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fruityvice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fruityvice
provider_slug: fruityvice
slug: fruityvice-domain-security
source_filename: fruityvice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fruityvice.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 09:39:58 2026 GMT\n  hsts: false\ndomains:\n- domain: fruityvice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fruityvice/refs/heads/main/security/fruityvice-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Food And Drink
- Public APIs
---
