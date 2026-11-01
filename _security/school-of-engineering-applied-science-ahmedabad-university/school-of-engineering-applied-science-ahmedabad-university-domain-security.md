---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ahduni.edu.in
  spf: true
hosts:
- cert_expires: Dec 27 09:35:02 2026 GMT
  host: ahduni.edu.in
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: School Of Engineering Applied Science Ahmedabad University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for School of Engineering & Applied Science, Ahmedabad University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: School of Engineering & Applied Science, Ahmedabad University
provider_slug: school-of-engineering-applied-science-ahmedabad-university
slug: school-of-engineering-applied-science-ahmedabad-university-domain-security
source_filename: school-of-engineering-applied-science-ahmedabad-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ahduni.edu.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 09:35:02 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: ahduni.edu.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/school-of-engineering-applied-science-ahmedabad-university/security/school-of-engineering-applied-science-ahmedabad-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Engineering
- HigherEducation
- India
- Research
---
