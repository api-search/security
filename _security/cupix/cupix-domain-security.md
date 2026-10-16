---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cupix.com
  spf: true
hosts:
- cert_expires: Nov 27 13:16:49 2026 GMT
  host: www.cupix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cupix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cupix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cupix
provider_slug: cupix
slug: cupix-domain-security
source_filename: cupix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cupix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 13:16:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cupix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cupix/refs/heads/main/security/cupix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Spatial Intelligence
- Digital Twin
- AI
---
