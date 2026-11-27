---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deepgent.net
  spf: true
hosts:
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: deepgent.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: deepgent-net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for deepgent-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: deepgent-net
provider_slug: deepgent-net
slug: deepgent-net-domain-security
source_filename: deepgent-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepgent.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deepgent.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/deepgent-net/security/deepgent-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chatbots
- E-Commerce
- Multi-Tenant
---
