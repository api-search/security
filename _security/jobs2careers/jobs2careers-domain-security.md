---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jobs2careers.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.jobs2careers.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Jobs2Careers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jobs2Careers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jobs2Careers
provider_slug: jobs2careers
slug: jobs2careers-domain-security
source_filename: jobs2careers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.jobs2careers.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: jobs2careers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobs2careers/refs/heads/main/security/jobs2careers-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Jobs
- Public APIs
---
