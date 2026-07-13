---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reed.co.uk
  spf: true
hosts:
- cert_expires: Sep 30 23:46:12 2026 GMT
  host: www.reed.co.uk
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Reed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reed
provider_slug: reed
slug: reed-domain-security
source_filename: reed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reed.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 23:46:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: reed.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reed/refs/heads/main/security/reed-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Jobs
- Public APIs
---
