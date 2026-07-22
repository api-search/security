---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blackore.ai
  spf: true
hosts:
- cert_expires: Oct  7 18:47:02 2026 GMT
  host: blackore.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Black Ore Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Ore Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Black Ore Technologies
provider_slug: black-ore-technologies
slug: black-ore-technologies-domain-security
source_filename: black-ore-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blackore.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:47:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blackore.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/black-ore-technologies/refs/heads/main/security/black-ore-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Financial Services
- Tax
- Accounting
- Fintech
- Automation
- Tax Preparation
---
