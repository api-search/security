---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: voxox.com
  spf: false
hosts:
- cert_expires: Dec 19 01:32:52 2026 GMT
  host: voxox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Voxox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voxox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Voxox
provider_slug: voxox
slug: voxox-domain-security
source_filename: voxox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voxox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 01:32:52 2026 GMT\n  hsts: false\ndomains:\n- domain: voxox.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voxox/refs/heads/main/security/voxox-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Telecommunications
- Communications
- Cloud Communications
- VoIP
- SMS
- Messaging
- CPaaS
---
