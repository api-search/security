---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:team-clf@monterail.com"
  - 0 issue "godaddy.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cooleaf.com
  spf: true
hosts:
- cert_expires: Sep 30 19:58:50 2026 GMT
  host: cooleaf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cooleaf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cooleaf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cooleaf
provider_slug: cooleaf
slug: cooleaf-domain-security
source_filename: cooleaf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cooleaf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:58:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cooleaf.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:team-clf@monterail.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooleaf/refs/heads/main/security/cooleaf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employee Engagement
- Employee Recognition
- Rewards
- Human Resources
- Employee Experience
- Surveys
- SaaS
---
