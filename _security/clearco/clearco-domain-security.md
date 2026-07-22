---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: clear.co
  spf: true
hosts:
- cert_expires: Oct  2 02:55:20 2026 GMT
  host: www.clear.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clearco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clearco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Clearco
provider_slug: clearco
slug: clearco-domain-security
source_filename: clearco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clear.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:55:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clear.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearco/refs/heads/main/security/clearco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Financing
- Ecommerce
- Working Capital
- Revenue-Based Financing
- Embedded Finance
---
