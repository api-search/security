---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: volunteerlocal.com
  spf: true
hosts:
- cert_expires: Dec 30 01:41:35 2026 GMT
  host: volunteerlocal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Volunteerlocal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VolunteerLocal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VolunteerLocal
provider_slug: volunteerlocal
slug: volunteerlocal-domain-security
source_filename: volunteerlocal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: volunteerlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 01:41:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: volunteerlocal.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/volunteerlocal/security/volunteerlocal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Volunteer Management
- Scheduling
- Communication
- Tracking
- Reporting
- Database
- Event Management
---
