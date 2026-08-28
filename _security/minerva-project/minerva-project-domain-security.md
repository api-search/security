---
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "trust-provider.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: minervaproject.com
  spf: true
hosts:
- cert_expires: Oct 15 16:44:57 2026 GMT
  host: www.minervaproject.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Minerva Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minerva Project, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Minerva Project
provider_slug: minerva-project
slug: minerva-project-domain-security
source_filename: minerva-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.minervaproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 16:44:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: minervaproject.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"trust-provider.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minerva-project/refs/heads/main/security/minerva-project-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Higher Education
- Learning Platform
- Active Learning
- Virtual Classroom
- Assessment
- Learning Analytics
---
