---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hub.xyz
  spf: true
hosts:
- cert_expires: Oct  4 11:13:14 2026 GMT
  host: hub.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.hub.xyz
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hub
provider_slug: hub
slug: hub-domain-security
source_filename: hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hub.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:13:14 2026 GMT\n  hsts: false\n- host: api.hub.xyz\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: hub.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hub/refs/heads/main/security/hub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Training Data
- Robotics
- Physical AI
- Datasets
- Data Infrastructure
- Annotation
- Multimodal
---
