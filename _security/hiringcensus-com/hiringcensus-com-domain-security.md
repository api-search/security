---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hiringcensus.com
  spf: true
hosts:
- cert_expires: Jan 24 10:25:05 2027 GMT
  host: hiringcensus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HiringCensus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiringCensus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HiringCensus
provider_slug: hiringcensus-com
slug: hiringcensus-com-domain-security
source_filename: hiringcensus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hiringcensus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 10:25:05 2027 GMT\n  hsts: false\ndomains:\n- domain: hiringcensus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hiringcensus-com/security/hiringcensus-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Job
- Data
- Hiring
---
