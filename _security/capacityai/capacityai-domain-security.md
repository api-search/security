---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: capacityai.io
  spf: true
hosts:
- cert_expires: Nov 30 21:28:41 2026 GMT
  host: capacityai.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capacityai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capacityai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Capacityai
provider_slug: capacityai
slug: capacityai-domain-security
source_filename: capacityai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capacityai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 21:28:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: capacityai.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capacityai/refs/heads/main/security/capacityai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
