---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hirevue.com
  spf: true
hosts:
- cert_expires: Sep 30 04:52:49 2026 GMT
  host: www.hirevue.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.hirevue.com
  https: false
- host: api.hirevue.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hirevue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HireVue, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HireVue
provider_slug: hirevue
slug: hirevue-domain-security
source_filename: hirevue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hirevue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 04:52:49 2026 GMT\n  hsts: false\n- host: developer.hirevue.com\n  https: false\n- host: api.hirevue.com\n  https: false\ndomains:\n- domain: hirevue.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hirevue/refs/heads/main/security/hirevue-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Video Interviewing
- Assessments
- AI Hiring
- Scheduling
- Conversational AI
- HR Tech
---
