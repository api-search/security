---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: autox.ai
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: www.autox.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AutoX
provider_slug: autox
slug: autox-domain-security
source_filename: autox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: autox.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autox/refs/heads/main/security/autox-domain-security.yml
summary_line: TLSv1.3
tags:
- Autonomous Driving
- AI
- Robotics
- Transportation
- San Jose
---
