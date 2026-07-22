---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tarefa.co
  spf: true
hosts:
- cert_expires: Sep 14 01:28:38 2026 GMT
  host: tarefa.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tarefa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tarefa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tarefa
provider_slug: tarefa
slug: tarefa-domain-security
source_filename: tarefa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tarefa.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:28:38 2026 GMT\n  hsts: false\ndomains:\n- domain: tarefa.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tarefa/refs/heads/main/security/tarefa-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Education
- EdTech
- E-Learning
- Online Courses
- STEM
- Mathematics
- Physics
- Chemistry
- Latin America
- Spanish
---
