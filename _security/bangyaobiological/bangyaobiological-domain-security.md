---
description: ''
domains:
- caa:
  - bangyao6689.websitecname.cn.
  dmarc: false
  dnssec: false
  domain: bangyaobio.com
  spf: false
hosts:
- host: www.bangyaobio.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.bangyao'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bangyaobiological Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bangyaobiological, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bangyaobiological
provider_slug: bangyaobiological
slug: bangyaobiological-domain-security
source_filename: bangyaobiological-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bangyaobio.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.bangyao'\n  hsts: null\ndomains:\n- domain: bangyaobio.com\n  dnssec: false\n  caa:\n  - bangyao6689.websitecname.cn.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bangyaobiological/refs/heads/main/security/bangyaobiological-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Biotechnology
- MedicalDevices
- Polymers
- Manufacturing
- China
---
