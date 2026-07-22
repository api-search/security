---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ethealthcare.com.cn
  spf: true
hosts:
- host: ethealthcare.com.cn
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Ethealthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ethealthcare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ethealthcare
provider_slug: ethealthcare
slug: ethealthcare-domain-security
source_filename: ethealthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ethealthcare.com.cn\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ethealthcare.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethealthcare/refs/heads/main/security/ethealthcare-domain-security.yml
summary_line: DMARC
tags:
- Company
- Healthcare
- Diagnostics
- Medical Devices
- In Vitro Diagnostics
- Immunoassay
- Life Sciences
---
