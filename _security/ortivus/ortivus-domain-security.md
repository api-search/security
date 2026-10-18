---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ortivus.com
  spf: true
hosts:
- cert_expires: Dec 13 07:30:48 2026 GMT
  host: www.ortivus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ortivus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ortivus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ortivus
provider_slug: ortivus
slug: ortivus-domain-security
source_filename: ortivus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ortivus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 07:30:48 2026 GMT\n  hsts: false\ndomains:\n- domain: ortivus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ortivus/refs/heads/main/security/ortivus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Emergency Services
- Digital Solutions
- Software-as-a-Service
---
