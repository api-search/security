---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ant-fa.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: ant-fa.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aante Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aante, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aante
provider_slug: aante
slug: aante-domain-security
source_filename: aante-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ant-fa.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ant-fa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aante/refs/heads/main/security/aante-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Industrial Automation
- Factory Automation
- Manufacturing
- Distribution
- E-Commerce
- Procurement
- Industrial Components
- China
---
