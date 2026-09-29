---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biryanibykilo.com
  spf: true
hosts:
- cert_expires: Apr  8 04:54:35 2027 GMT
  host: biryanibykilo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biryanibykilo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biryanibykilo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biryanibykilo
provider_slug: biryanibykilo
slug: biryanibykilo-domain-security
source_filename: biryanibykilo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biryanibykilo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 04:54:35 2027 GMT\n  hsts: false\ndomains:\n- domain: biryanibykilo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biryanibykilo/refs/heads/main/security/biryanibykilo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food
- Delivery
- Biryani
- India
---
