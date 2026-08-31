---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: answers.com
  spf: true
hosts:
- cert_expires: Apr  5 19:50:17 2027 GMT
  host: www.answers.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Answerscom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Answers.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Answers.com
provider_slug: answerscom
slug: answerscom-domain-security
source_filename: answerscom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.answers.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  5 19:50:17 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: answers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/answerscom/refs/heads/main/security/answerscom-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Question and Answer
- Reference
- Knowledge
- Content
- Consumer
- Education
---
