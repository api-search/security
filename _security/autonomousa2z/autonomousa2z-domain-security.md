---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: autoa2z.ai
  spf: true
hosts:
- cert_expires: Mar 31 23:59:59 2027 GMT
  host: www.autoa2z.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autonomousa2Z Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autonomousa2z, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Autonomousa2z
provider_slug: autonomousa2z
slug: autonomousa2z-domain-security
source_filename: autonomousa2z-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autoa2z.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: autoa2z.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autonomousa2z/refs/heads/main/security/autonomousa2z-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Autonomous Vehicles
- AI
- Mobility
- Korea
---
