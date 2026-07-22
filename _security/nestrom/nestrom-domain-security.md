---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nestrom.com
  spf: true
hosts:
- cert_expires: Sep  8 16:28:04 2026 GMT
  host: nestrom.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nestrom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nestrom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nestrom
provider_slug: nestrom
slug: nestrom-domain-security
source_filename: nestrom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nestrom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 16:28:04 2026 GMT\n  hsts: null\ndomains:\n- domain: nestrom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nestrom/refs/heads/main/security/nestrom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
