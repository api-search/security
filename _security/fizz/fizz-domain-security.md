---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fizz.social
  spf: true
hosts:
- cert_expires: Sep 11 06:40:52 2026 GMT
  host: fizz.social
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fizz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fizz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fizz
provider_slug: fizz
slug: fizz-domain-security
source_filename: fizz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fizz.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:40:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fizz.social\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fizz/refs/heads/main/security/fizz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social
- Social Networking
- Community
- Campus
- Higher Education
- Students
- Consumer
- Mobile
- Marketplace
---
