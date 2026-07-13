---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amdoren.com
  spf: false
hosts:
- cert_expires: Aug 20 06:01:29 2026 GMT
  host: www.amdoren.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amdoren Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amdoren, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Amdoren
provider_slug: amdoren
slug: amdoren-domain-security
source_filename: amdoren-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amdoren.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:01:29 2026 GMT\n  hsts: false\ndomains:\n- domain: amdoren.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amdoren/refs/heads/main/security/amdoren-domain-security.yml
summary_line: TLSv1.3
tags:
- Currency Exchange
- Public APIs
---
