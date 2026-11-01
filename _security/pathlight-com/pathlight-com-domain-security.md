---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pathlight.ai
  spf: false
hosts:
- cert_expires: Dec 31 19:46:22 2026 GMT
  host: pathlight.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pathlight Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Echo AI (fka Pathlight), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Echo AI (fka Pathlight)
provider_slug: pathlight-com
slug: pathlight-com-domain-security
source_filename: pathlight-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pathlight.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 19:46:22 2026 GMT\n  hsts: null\ndomains:\n- domain: pathlight.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pathlight-com/security/pathlight-com-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- Communication
- SpeechRecognition
- Analytics
- Enterprise
---
