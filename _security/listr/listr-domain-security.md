---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: listr.com
  spf: true
hosts:
- cert_expires: Nov 16 05:55:33 2026 GMT
  host: listr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Listr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiSTR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LiSTR
provider_slug: listr
slug: listr-domain-security
source_filename: listr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 05:55:33 2026 GMT\n  hsts: null\ndomains:\n- domain: listr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listr/refs/heads/main/security/listr-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
