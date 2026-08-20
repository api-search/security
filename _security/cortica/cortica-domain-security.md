---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cortica.com
  spf: false
hosts:
- cert_expires: Oct 23 13:41:48 2026 GMT
  host: cortica.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cortica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cortica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cortica
provider_slug: cortica
slug: cortica-domain-security
source_filename: cortica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cortica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 13:41:48 2026 GMT\n  hsts: false\ndomains:\n- domain: cortica.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cortica/refs/heads/main/security/cortica-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Computer-Vision
- Machine-Learning
- Autonomous Systems
- Venture Builder
- Israel
- Deep Tech
---
