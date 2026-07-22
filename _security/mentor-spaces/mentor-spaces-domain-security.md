---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mentorspaces.com
  spf: false
hosts:
- cert_expires: Sep 27 02:48:32 2026 GMT
  host: mentorspaces.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mentor Spaces Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mentor Spaces, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Mentor Spaces
provider_slug: mentor-spaces
slug: mentor-spaces-domain-security
source_filename: mentor-spaces-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mentorspaces.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 02:48:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mentorspaces.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mentor-spaces/refs/heads/main/security/mentor-spaces-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mentorship
- Nonprofits
- Education
- Volunteering
- Impact Measurement
- Workforce Development
---
