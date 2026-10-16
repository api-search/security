---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liferaft.co
  spf: true
hosts:
- cert_expires: Nov 24 12:45:09 2026 GMT
  host: www.liferaft.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Liferaft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liferaft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Liferaft
provider_slug: liferaft
slug: liferaft-domain-security
source_filename: liferaft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liferaft.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 12:45:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: liferaft.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liferaft/refs/heads/main/security/liferaft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Benefits
- Insurance
- SaaS
---
