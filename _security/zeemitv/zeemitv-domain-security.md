---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zeemi.tv
  spf: true
hosts:
- cert_expires: Sep 23 03:31:02 2026 GMT
  host: zeemi.tv
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zeemitv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeemi.tv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Zeemi.tv
provider_slug: zeemitv
slug: zeemitv-domain-security
source_filename: zeemitv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeemi.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 03:31:02 2026 GMT\n  hsts: null\ndomains:\n- domain: zeemi.tv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeemitv/refs/heads/main/security/zeemitv-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
