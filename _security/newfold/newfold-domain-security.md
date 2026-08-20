---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: newfold.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hiive.cloud
  spf: true
hosts:
- cert_expires: Nov 10 13:12:35 2026 GMT
  host: newfold.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 06:30:33 2026 GMT
  host: hiive.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newfold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newfold, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Newfold
provider_slug: newfold
slug: newfold-domain-security
source_filename: newfold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newfold.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 13:12:35 2026 GMT\n  hsts: null\n- host: hiive.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:30:33 2026 GMT\n  hsts: null\ndomains:\n- domain: newfold.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hiive.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newfold/refs/heads/main/security/newfold-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Web Hosting
- Domains
- Web Presence
- Website Builder
- Digital Marketing
- Small Business
- WordPress
- Open-Source
- MCP
- E-Commerce
---
