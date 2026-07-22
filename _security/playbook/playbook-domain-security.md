---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: get-playbook.com
  spf: true
hosts:
- cert_expires: Oct  2 17:01:15 2026 GMT
  host: get-playbook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Playbook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Playbook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Playbook
provider_slug: playbook
slug: playbook-domain-security
source_filename: playbook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: get-playbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:01:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: get-playbook.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playbook/refs/heads/main/security/playbook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Career Development
- Community
- Education
- Women in Leadership
- Professional Networking
- Masterclasses
---
