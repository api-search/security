---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abbeypost.com
  spf: true
hosts:
- cert_expires: Sep  6 07:49:11 2026 GMT
  host: abbeypost.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abbeypost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abbeypost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Abbeypost
provider_slug: abbeypost
slug: abbeypost-domain-security
source_filename: abbeypost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abbeypost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 07:49:11 2026 GMT\n  hsts: null\ndomains:\n- domain: abbeypost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abbeypost/refs/heads/main/security/abbeypost-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
