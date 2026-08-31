---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sparkneuro.com
  spf: true
hosts:
- cert_expires: Oct 25 20:03:40 2026 GMT
  host: sparkneuro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spark Neuro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPARK Neuro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SPARK Neuro
provider_slug: spark-neuro
slug: spark-neuro-domain-security
source_filename: spark-neuro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sparkneuro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 20:03:40 2026 GMT\n  hsts: false\ndomains:\n- domain: sparkneuro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spark-neuro/refs/heads/main/security/spark-neuro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Neuroscience
- Neurotechnology
- Healthcare
- Medical Devices
- EEG
- Artificial Intelligence
- Diagnostics
- Clinical Trials
- Advertising
---
