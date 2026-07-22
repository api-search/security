---
description: ''
domains:
- caa:
  - 0 iodef "mailto:info@techiematter.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: techiematter.com
  spf: true
hosts:
- cert_expires: Oct 19 08:50:28 2026 GMT
  host: techiematter.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Techiematter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TechieMatter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TechieMatter
provider_slug: techiematter
slug: techiematter-domain-security
source_filename: techiematter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: techiematter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 08:50:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: techiematter.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:info@techiematter.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/techiematter/refs/heads/main/security/techiematter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruitment
- Hiring
- Talent
- Technical Assessment
- Onboarding
- HR Tech
---
