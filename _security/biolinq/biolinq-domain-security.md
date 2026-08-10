---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biolinq.com
  spf: true
hosts:
- cert_expires: Sep 30 00:26:45 2026 GMT
  host: www.biolinq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biolinq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biolinq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biolinq
provider_slug: biolinq
slug: biolinq-domain-security
source_filename: biolinq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biolinq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:26:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: biolinq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biolinq/refs/heads/main/security/biolinq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Digital Health
- Medical Devices
- Wearables
- Biosensors
- Continuous Glucose Monitoring
- Diabetes
---
