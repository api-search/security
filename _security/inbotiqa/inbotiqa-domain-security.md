---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inbotiqa.com
  spf: true
hosts:
- cert_expires: Oct  8 19:24:45 2026 GMT
  host: inbotiqa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inbotiqa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INBOTIQA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: INBOTIQA
provider_slug: inbotiqa
slug: inbotiqa-domain-security
source_filename: inbotiqa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inbotiqa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:24:45 2026 GMT\n  hsts: false\ndomains:\n- domain: inbotiqa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inbotiqa/refs/heads/main/security/inbotiqa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Email
- Shared Inbox
- Workflow
- Fintech
- Financial Services
- Machine Learning
- Productivity
- Collaboration
- SaaS
---
