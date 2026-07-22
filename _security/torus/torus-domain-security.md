---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: usetorus.com
  spf: true
hosts:
- cert_expires: Sep  4 19:09:37 2026 GMT
  host: usetorus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Torus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Torus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Torus
provider_slug: torus
slug: torus-domain-security
source_filename: torus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usetorus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 19:09:37 2026 GMT\n  hsts: false\ndomains:\n- domain: usetorus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/torus/refs/heads/main/security/torus-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Agents
- Engineering
- Construction
- Capital Projects
- Infrastructure
- Document Intelligence
---
