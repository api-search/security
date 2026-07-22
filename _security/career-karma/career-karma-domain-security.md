---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: careerkarma.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: careerkarma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Career Karma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Career Karma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Career Karma
provider_slug: career-karma
slug: career-karma-domain-security
source_filename: career-karma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: careerkarma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: careerkarma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/career-karma/refs/heads/main/security/career-karma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Education
- Career Training
- Bootcamps
- EdTech
- Program Matching
---
