---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: merlyn.org
  spf: true
hosts:
- cert_expires: Oct 22 00:52:49 2026 GMT
  host: www.merlyn.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Merlyn Mind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merlyn Mind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Merlyn Mind
provider_slug: merlyn-mind
slug: merlyn-mind-domain-security
source_filename: merlyn-mind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.merlyn.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 00:52:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: merlyn.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merlyn-mind/refs/heads/main/security/merlyn-mind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Education
- EdTech
- K-12
- Large Language Models
- Voice Assistant
- Classroom Technology
- Machine Learning
- Responsible AI
---
