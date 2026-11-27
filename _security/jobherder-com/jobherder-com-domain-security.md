---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jobherder.com
  spf: true
hosts:
- cert_expires: Feb  3 16:47:13 2027 GMT
  host: jobherder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jobherder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jobherder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Jobherder
provider_slug: jobherder-com
slug: jobherder-com-domain-security
source_filename: jobherder-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobherder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 16:47:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jobherder.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jobherder-com/security/jobherder-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Job Search
- Artificial Intelligence
- Automation
- Privacy
- Careers
---
