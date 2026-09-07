---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 4gclinical.com
  spf: true
hosts:
- cert_expires: Nov 17 20:46:48 2026 GMT
  host: www.4gclinical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.4gclinical.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 4Gclinical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4G Clinical, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 4G Clinical
provider_slug: 4gclinical
slug: 4gclinical-domain-security
source_filename: 4gclinical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.4gclinical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 20:46:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.4gclinical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: 4gclinical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4gclinical/refs/heads/main/security/4gclinical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Clinical Trials
- Life Sciences
- Randomization
- Trial Supply Management
- RTSM
- Clinical Supply Chain
- Pharmaceutical
- Healthcare
- Forecasting
- Company
---
