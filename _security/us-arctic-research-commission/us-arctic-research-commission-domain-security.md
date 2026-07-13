---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arctic.gov
  spf: true
hosts:
- cert_expires: Sep 29 05:01:22 2026 GMT
  host: www.arctic.gov
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Arctic Research Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Arctic Research Commission, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Arctic Research Commission
provider_slug: us-arctic-research-commission
slug: us-arctic-research-commission-domain-security
source_filename: us-arctic-research-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arctic.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:01:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: arctic.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-arctic-research-commission/refs/heads/main/security/us-arctic-research-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Arctic Research
- Federal Government
- Climate Change
- Research Policy
- Advisory Commission
- Arctic
- Environmental Science
---
