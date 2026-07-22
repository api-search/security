---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: makethedot.com
  spf: true
hosts:
- cert_expires: Oct  1 03:15:33 2026 GMT
  host: makethedot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Make The Dot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Make the Dot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Make the Dot
provider_slug: make-the-dot
slug: make-the-dot-domain-security
source_filename: make-the-dot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makethedot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:15:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: makethedot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/make-the-dot/refs/heads/main/security/make-the-dot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fashion
- Apparel
- Product Development
- PLM
- Design
- Merchandising
- Artificial Intelligence
- SaaS
- Collaboration
---
