---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: signup.com
  spf: true
hosts:
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: signup.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Signup Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SignUp.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SignUp.com
provider_slug: signup-com
slug: signup-com-domain-security
source_filename: signup-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: signup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/signup-com/security/signup-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SaaS
- Scheduling
- Volunteer
- Education
- Nonprofit
---
