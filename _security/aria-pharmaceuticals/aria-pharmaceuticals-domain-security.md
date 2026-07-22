---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ariapharmaceuticals.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: ariapharmaceuticals.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aria Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aria Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aria Pharmaceuticals
provider_slug: aria-pharmaceuticals
slug: aria-pharmaceuticals-domain-security
source_filename: aria-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ariapharmaceuticals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ariapharmaceuticals.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aria-pharmaceuticals/refs/heads/main/security/aria-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Drug Discovery
- Artificial Intelligence
- Biotechnology
- Healthcare
- Life Sciences
---
