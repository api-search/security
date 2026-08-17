---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onecommand.com
  spf: true
hosts:
- cert_expires: Sep 14 16:47:08 2026 GMT
  host: www.onecommand.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onecommand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneCommand, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OneCommand
provider_slug: onecommand
slug: onecommand-domain-security
source_filename: onecommand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onecommand.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:47:08 2026 GMT\n  hsts: null\ndomains:\n- domain: onecommand.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onecommand/refs/heads/main/security/onecommand-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Marketing
- Customer Loyalty
- Marketing Automation
- CRM
- Dealership
---
