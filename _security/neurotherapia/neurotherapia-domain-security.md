---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neurotherapia.com
  spf: false
hosts:
- cert_expires: Nov 19 19:51:06 2026 GMT
  host: www.neurotherapia.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neurotherapia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NeuroTherapia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: NeuroTherapia
provider_slug: neurotherapia
slug: neurotherapia-domain-security
source_filename: neurotherapia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neurotherapia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 19:51:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: neurotherapia.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neurotherapia/refs/heads/main/security/neurotherapia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Health
- Clinical Trials
- Neuroscience
- Drug Discovery
- Alzheimer's Disease
- Company
---
