---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shelby.tv
  spf: true
hosts:
- cert_expires: Sep 18 12:27:34 2026 GMT
  host: shelby.tv
  hsts: true
  hsts_max_age: 15552001
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shelbytv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shelby.tv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Shelby.tv
provider_slug: shelbytv
slug: shelbytv-domain-security
source_filename: shelbytv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shelby.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 12:27:34 2026 GMT\n  hsts: true\n  hsts_max_age: 15552001\ndomains:\n- domain: shelby.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shelbytv/refs/heads/main/security/shelbytv-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Video
- Social
- Video Discovery
- Media
- Defunct
---
