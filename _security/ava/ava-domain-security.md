---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: meetava.com
  spf: true
hosts:
- cert_expires: Aug 22 06:24:38 2026 GMT
  host: www.meetava.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ava Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ava, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ava
provider_slug: ava
slug: ava-domain-security
source_filename: ava-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meetava.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:24:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meetava.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ava/refs/heads/main/security/ava-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Credit Building
- Consumer Finance
- Credit Score
- Personal Finance
- Lending
- Mobile App
---
