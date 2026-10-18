---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: collectivex.ai
  spf: false
hosts:
- cert_expires: Nov 28 15:41:59 2026 GMT
  host: www.collectivex.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Collectivex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collectivex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Collectivex
provider_slug: collectivex
slug: collectivex-domain-security
source_filename: collectivex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.collectivex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 15:41:59 2026 GMT\n  hsts: false\ndomains:\n- domain: collectivex.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collectivex/refs/heads/main/security/collectivex-domain-security.yml
summary_line: TLSv1.3
tags:
- Healthcare
- Artificial Intelligence
- Diagnostics
- Research
- Platform
- Company
---
