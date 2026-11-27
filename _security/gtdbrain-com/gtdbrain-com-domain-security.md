---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gtdbrain.com
  spf: true
hosts:
- cert_expires: Dec 18 22:21:59 2026 GMT
  host: gtdbrain.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GTD Brain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GTD Brain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GTD Brain
provider_slug: gtdbrain-com
slug: gtdbrain-com-domain-security
source_filename: gtdbrain-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gtdbrain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 22:21:59 2026 GMT\n  hsts: false\ndomains:\n- domain: gtdbrain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gtdbrain-com/security/gtdbrain-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Productivity
- GTD
- Artificial Intelligence
- Task Management
- Cross-Platform
---
