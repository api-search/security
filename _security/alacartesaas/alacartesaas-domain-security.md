---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alacartesaas.com
  spf: true
hosts:
- cert_expires: Dec 23 08:20:54 2026 GMT
  host: alacartesaas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alacartesaas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneBill Utilities, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OneBill Utilities
provider_slug: alacartesaas
slug: alacartesaas-domain-security
source_filename: alacartesaas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alacartesaas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 08:20:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alacartesaas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alacartesaas/refs/heads/main/security/alacartesaas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Comparison
- SaaS
- Ireland
---
