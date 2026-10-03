---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bart.gov
  spf: true
hosts:
- cert_expires: Nov 19 01:31:41 2026 GMT
  host: www.bart.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bart
provider_slug: bart
slug: bart-domain-security
source_filename: bart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bart.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 01:31:41 2026 GMT\n  hsts: false\ndomains:\n- domain: bart.gov\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bart/refs/heads/main/security/bart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transit
- Public Transport
- Real-Time Data
- Bay Area
---
