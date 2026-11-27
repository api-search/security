---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jobcrawls.com
  spf: false
hosts:
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: jobcrawls.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JobCrawls Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JobCrawls, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: JobCrawls
provider_slug: jobcrawls-com
slug: jobcrawls-com-domain-security
source_filename: jobcrawls-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobcrawls.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: jobcrawls.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/jobcrawls-com/security/jobcrawls-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Job Search
- Finland
- Remote Jobs
- Data Reuse
- Technology
---
