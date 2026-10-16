---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: connexusinc.org
  spf: false
hosts:
- cert_expires: Mar 27 14:04:05 2027 GMT
  host: connexusinc.org
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connexus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connexus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Connexus
provider_slug: connexus
slug: connexus-domain-security
source_filename: connexus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connexusinc.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 27 14:04:05 2027 GMT\n  hsts: false\ndomains:\n- domain: connexusinc.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connexus/refs/heads/main/security/connexus-domain-security.yml
summary_line: TLSv1.2
tags:
- Nonprofit
- Healthcare
- Social Services
- Community Support
- Tennessee
---
