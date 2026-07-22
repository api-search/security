---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flatiron.com
  spf: true
hosts:
- cert_expires: Sep 19 20:25:40 2026 GMT
  host: flatiron.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flatiron Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flatiron Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flatiron Health
provider_slug: flatiron-health
slug: flatiron-health-domain-security
source_filename: flatiron-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flatiron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:25:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flatiron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flatiron-health/refs/heads/main/security/flatiron-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Oncology
- Real-World Data
- Real-World Evidence
- Clinical Trials
- Life Sciences
- Electronic Health Records
---
