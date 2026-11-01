---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jobzmall.com
  spf: true
hosts:
- cert_expires: Jan 10 10:43:44 2027 GMT
  host: www.jobzmall.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jobzmall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JobzMall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: JobzMall
provider_slug: jobzmall
slug: jobzmall-domain-security
source_filename: jobzmall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jobzmall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 10:43:44 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: jobzmall.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/jobzmall/security/jobzmall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- video
- talent
- marketplace
- hiring
- resumes
---
