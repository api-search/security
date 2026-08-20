---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: neuroflow.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: neuroflowlive.com
  spf: false
hosts:
- cert_expires: Sep 13 18:57:39 2026 GMT
  host: www.neuroflow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: neuroflowlive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neuroflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NeuroFlow, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NeuroFlow
provider_slug: neuroflow
slug: neuroflow-domain-security
source_filename: neuroflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neuroflow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:57:39 2026 GMT\n  hsts: false\n- host: neuroflowlive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: neuroflow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: neuroflowlive.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neuroflow/refs/heads/main/security/neuroflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Behavioral Health
- Healthcare
- Mental Health
- Digital Health
- Care Coordination
- Health Analytics
- EHR Integration
---
