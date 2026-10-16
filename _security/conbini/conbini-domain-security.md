---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: conbini.com
  spf: true
hosts:
- cert_expires: Nov 16 04:28:36 2026 GMT
  host: conbini.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Conbini Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conbini, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Conbini
provider_slug: conbini
slug: conbini-domain-security
source_filename: conbini-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conbini.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 04:28:36 2026 GMT\n  hsts: false\ndomains:\n- domain: conbini.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conbini/refs/heads/main/security/conbini-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Retail
- E-commerce
- Japan
- Snacks
---
