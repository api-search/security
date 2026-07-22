---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: peopleonehealth.com
  spf: true
hosts:
- cert_expires: Oct 11 06:25:16 2026 GMT
  host: peopleonehealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peopleone Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PeopleOne Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PeopleOne Health
provider_slug: peopleone-health
slug: peopleone-health-domain-security
source_filename: peopleone-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peopleonehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 06:25:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: peopleonehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopleone-health/refs/heads/main/security/peopleone-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Healthcare
- Primary Care
- Value-Based Care
- Employer Benefits
- Digital Health
---
