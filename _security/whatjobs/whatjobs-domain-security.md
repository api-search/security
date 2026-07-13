---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: whatjobs.com
  spf: true
hosts:
- cert_expires: Sep 12 08:01:18 2026 GMT
  host: www.whatjobs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whatjobs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WhatJobs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WhatJobs
provider_slug: whatjobs
slug: whatjobs-domain-security
source_filename: whatjobs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.whatjobs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 08:01:18 2026 GMT\n  hsts: false\ndomains:\n- domain: whatjobs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whatjobs/refs/heads/main/security/whatjobs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Jobs
- Public APIs
---
