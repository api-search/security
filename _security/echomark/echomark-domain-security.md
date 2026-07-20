---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: echomark.com
  spf: true
hosts:
- cert_expires: Oct 16 08:02:49 2026 GMT
  host: echomark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Echomark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EchoMark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EchoMark
provider_slug: echomark
slug: echomark-domain-security
source_filename: echomark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: echomark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 08:02:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: echomark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echomark/refs/heads/main/security/echomark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Information Security
- Forensic Watermarking
- Insider Threat
- Data Loss Prevention
- Leak Detection
---
