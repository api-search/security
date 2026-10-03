---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avatier.com
  spf: true
hosts:
- cert_expires: Nov 19 06:28:32 2026 GMT
  host: www.avatier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avatier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avatier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Avatier
provider_slug: avatier
slug: avatier-domain-security
source_filename: avatier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avatier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 06:28:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avatier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avatier/refs/heads/main/security/avatier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity
- Access Management
- Artificial Intelligence
- Cloud
- Enterprise
---
