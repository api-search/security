---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jobsforaiagents.com
  spf: true
hosts:
- cert_expires: Dec 13 14:39:56 2026 GMT
  host: jobsforaiagents.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jobsforaiagents Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jobsforaiagents-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: jobsforaiagents-com
provider_slug: jobsforaiagents-com
slug: jobsforaiagents-com-domain-security
source_filename: jobsforaiagents-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobsforaiagents.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 14:39:56 2026 GMT\n  hsts: null\ndomains:\n- domain: jobsforaiagents.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jobsforaiagents-com/security/jobsforaiagents-com-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
---
