---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cubyn.com
  spf: false
hosts:
- cert_expires: Dec 16 08:58:02 2026 GMT
  host: www.cubyn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cubyn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cubyn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cubyn
provider_slug: cubyn
slug: cubyn-domain-security
source_filename: cubyn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cubyn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 08:58:02 2026 GMT\n  hsts: false\ndomains:\n- domain: cubyn.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubyn/refs/heads/main/security/cubyn-domain-security.yml
summary_line: TLSv1.3
tags:
- Logistics
- Fulfillment
- E-Commerce
- Paris
---
