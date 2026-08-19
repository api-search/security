---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shadow.tech
  spf: true
hosts:
- cert_expires: Nov 12 15:31:11 2026 GMT
  host: shadow.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 02:14:54 2026 GMT
  host: gpu-instances.shadow.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: auth.frsbg01.os.shadow.tech
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Shadow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shadow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Shadow
provider_slug: shadow
slug: shadow-domain-security
source_filename: shadow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shadow.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 15:31:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gpu-instances.shadow.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 02:14:54 2026 GMT\n  hsts: false\n- host: auth.frsbg01.os.shadow.tech\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: shadow.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shadow/refs/heads/main/security/shadow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Computing
- GPU
- Cloud Gaming
- Infrastructure
- OpenStack
- AI Infrastructure
- Compute
- Storage
- Europe
---
