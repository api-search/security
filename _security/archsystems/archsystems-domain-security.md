---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: archsystems.com
  spf: true
hosts:
- cert_expires: Dec  1 06:56:06 2026 GMT
  host: archsystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Archsystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archsystems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Archsystems
provider_slug: archsystems
slug: archsystems-domain-security
source_filename: archsystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: archsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 06:56:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: archsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archsystems/refs/heads/main/security/archsystems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Architecture
- Interior Design
- Materials
- Manufacturing
- Sustainable
- Company
---
