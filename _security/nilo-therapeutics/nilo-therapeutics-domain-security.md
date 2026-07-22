---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nilotx.com
  spf: true
hosts:
- cert_expires: Sep 30 19:49:38 2026 GMT
  host: www.nilotx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nilo Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nilo Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nilo Therapeutics
provider_slug: nilo-therapeutics
slug: nilo-therapeutics-domain-security
source_filename: nilo-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nilotx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:49:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nilotx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nilo-therapeutics/refs/heads/main/security/nilo-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Therapeutics
- Immunology
- Neuroscience
- Drug Discovery
- Pharmaceuticals
- Healthcare
---
