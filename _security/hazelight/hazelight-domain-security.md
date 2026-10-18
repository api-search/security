---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hazelight.se
  spf: true
hosts:
- cert_expires: Nov 25 12:48:28 2026 GMT
  host: hazelight.se
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 07:11:07 2026 GMT
  host: store.hazelight.se
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Hazelight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hazelight, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hazelight
provider_slug: hazelight
slug: hazelight-domain-security
source_filename: hazelight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hazelight.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 12:48:28 2026 GMT\n  hsts: false\n- host: store.hazelight.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 07:11:07 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: hazelight.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hazelight/refs/heads/main/security/hazelight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Gaming
- Video Games
- Cooperative
- Sweden
- Studio
---
