---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getcanopy.co
  spf: true
hosts:
- cert_expires: Dec 27 17:48:02 2026 GMT
  host: getcanopy.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Canopyb4C1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canopyb4c1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Canopyb4c1
provider_slug: canopyb4c1
slug: canopyb4c1-domain-security
source_filename: canopyb4c1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getcanopy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 17:48:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: getcanopy.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canopyb4c1/refs/heads/main/security/canopyb4c1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
