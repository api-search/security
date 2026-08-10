---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: valohealth.com
  spf: true
hosts:
- cert_expires: Oct 25 04:01:03 2026 GMT
  host: www.valohealth.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valo Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valo Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Valo Health
provider_slug: valo-health
slug: valo-health-domain-security
source_filename: valo-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.valohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 04:01:03 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: valohealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valo-health/refs/heads/main/security/valo-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Drug Discovery
- Life Sciences
- Artificial Intelligence
- Machine Learning
- Pharmaceuticals
- Health
- Research
---
