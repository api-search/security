---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ranger.net
  spf: true
hosts:
- cert_expires: Sep 30 05:06:57 2026 GMT
  host: www.ranger.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ranger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ranger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ranger
provider_slug: ranger
slug: ranger-domain-security
source_filename: ranger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ranger.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:06:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ranger.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ranger/refs/heads/main/security/ranger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Quality Assurance
- Testing
- Browser Automation
- Artificial Intelligence
- Agents
- Developer Tools
- DevOps
- CLI
---
