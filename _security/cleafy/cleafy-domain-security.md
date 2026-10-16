---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cleafy.com
  spf: true
hosts:
- cert_expires: Dec  5 22:14:58 2026 GMT
  host: www.cleafy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cleafy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cleafy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cleafy
provider_slug: cleafy
slug: cleafy-domain-security
source_filename: cleafy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cleafy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 22:14:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cleafy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleafy/refs/heads/main/security/cleafy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Fraud Prevention
- Banking
- AI
---
