---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bootc.dev
  spf: false
hosts:
- cert_expires: Sep  5 04:32:20 2026 GMT
  host: bootc.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bootc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bootc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bootc
provider_slug: bootc
slug: bootc-domain-security
source_filename: bootc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bootc.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 04:32:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: bootc.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bootc/refs/heads/main/security/bootc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CNCF
- Container Images
- Infrastructure
- OCI
- Open Source
- Operating Systems
- System Updates
---
