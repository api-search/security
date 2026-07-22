---
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moderncampus.com
  spf: true
hosts:
- cert_expires: Sep 25 14:49:35 2026 GMT
  host: moderncampus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Presence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Presence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Presence
provider_slug: presence
slug: presence-domain-security
source_filename: presence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moderncampus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:49:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: moderncampus.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/presence/refs/heads/main/security/presence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Higher Education
- Student Engagement
- EdTech
- Campus Life
- Co-Curricular
- SaaS
---
