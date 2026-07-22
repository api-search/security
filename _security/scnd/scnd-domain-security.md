---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: scnd.com
  spf: true
hosts:
- cert_expires: Oct  2 19:56:01 2026 GMT
  host: www.scnd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scnd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Second (scnd), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Second (scnd)
provider_slug: scnd
slug: scnd-domain-security
source_filename: scnd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scnd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:56:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scnd.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scnd/refs/heads/main/security/scnd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Marketplace
- Services
- Vendor Management
- Payments
- OAuth
- SaaS
- Procurement
---
