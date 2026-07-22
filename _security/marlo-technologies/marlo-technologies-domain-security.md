---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: marlo.co
  spf: true
hosts:
- cert_expires: Sep 20 23:58:43 2026 GMT
  host: www.marlo.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marlo Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marlo Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Marlo Technologies
provider_slug: marlo-technologies
slug: marlo-technologies-domain-security
source_filename: marlo-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marlo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:58:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marlo.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marlo-technologies/refs/heads/main/security/marlo-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Maritime
- Shipping
- ERP
- Fintech
- Banking
- Compliance
- Logistics
---
