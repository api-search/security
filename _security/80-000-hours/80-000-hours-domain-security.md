---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 80000hours.org
  spf: true
hosts:
- cert_expires: Sep  6 23:45:36 2026 GMT
  host: 80000hours.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 80 000 Hours Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 80,000 Hours, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 80,000 Hours
provider_slug: 80-000-hours
slug: 80-000-hours-domain-security
source_filename: 80-000-hours-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 80000hours.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:45:36 2026 GMT\n  hsts: false\ndomains:\n- domain: 80000hours.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/80-000-hours/refs/heads/main/security/80-000-hours-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Nonprofit
- Careers
- Career Advice
- Effective Altruism
- Job Board
- AI Safety
- Research
- Podcast
- Content
---
