---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: alongside.com
  spf: true
hosts:
- cert_expires: Feb 27 15:19:27 2027 GMT
  host: app.alongside.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alongsidefinance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alongsidefinance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alongsidefinance
provider_slug: alongsidefinance
slug: alongsidefinance-domain-security
source_filename: alongsidefinance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.alongside.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 27 15:19:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alongside.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alongsidefinance/refs/heads/main/security/alongsidefinance-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Finance
- PersonalFinance
- Budgeting
- Investment
- SaaS
---
