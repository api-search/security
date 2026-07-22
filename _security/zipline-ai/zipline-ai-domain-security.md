---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zipline.ai
  spf: true
hosts:
- cert_expires: Sep 29 18:42:45 2026 GMT
  host: zipline.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zipline Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zipline Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Zipline Ai
provider_slug: zipline-ai
slug: zipline-ai-domain-security
source_filename: zipline-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zipline.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:42:45 2026 GMT\n  hsts: false\ndomains:\n- domain: zipline.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zipline-ai/refs/heads/main/security/zipline-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
