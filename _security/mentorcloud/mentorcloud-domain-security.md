---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mentorcloud.com
  spf: true
hosts:
- cert_expires: Sep 12 17:57:31 2026 GMT
  host: mentorcloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mentorcloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MentorCloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MentorCloud
provider_slug: mentorcloud
slug: mentorcloud-domain-security
source_filename: mentorcloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mentorcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 17:57:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mentorcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mentorcloud/refs/heads/main/security/mentorcloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mentoring
- Mentorship
- Talent Development
- Employee Engagement
- Learning and Development
- Human Resources
- SaaS
- DEI
- Higher Education
---
