---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: granthika.com
  spf: true
hosts:
- cert_expires: Aug 26 05:34:51 2026 GMT
  host: www.granthika.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Granthika Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Granthika, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Granthika
provider_slug: granthika
slug: granthika-domain-security
source_filename: granthika-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.granthika.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 05:34:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: granthika.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granthika/refs/heads/main/security/granthika-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Writing Software
- Semantic Editor
- Authoring
- Productivity
- Fiction
- MCP
---
