---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: katoomi.com
  spf: true
hosts:
- cert_expires: Nov 22 07:41:05 2026 GMT
  host: katoomi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Katoomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Katoomi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Katoomi
provider_slug: katoomi
slug: katoomi-domain-security
source_filename: katoomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: katoomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 07:41:05 2026 GMT\n  hsts: false\ndomains:\n- domain: katoomi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/katoomi/refs/heads/main/security/katoomi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Integration
- NetSuite
- SaaS
- eCommerce
---
