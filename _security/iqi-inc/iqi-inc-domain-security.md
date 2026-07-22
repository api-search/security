---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: iqi-inc.com
  spf: true
hosts:
- host: www.iqi-inc.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.iqi-inc'
kind: domain-security
layout: security
method: probed
name: Iqi Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IQI Inc (Beijing AIQI Technology), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: IQI Inc (Beijing AIQI Technology)
provider_slug: iqi-inc
slug: iqi-inc-domain-security
source_filename: iqi-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iqi-inc.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.iqi-inc'\n  hsts: null\ndomains:\n- domain: iqi-inc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iqi-inc/refs/heads/main/security/iqi-inc-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Robotics
- Smart Hardware
- Building Blocks
- Consumer Electronics
- Toys
- Xiaomi Ecosystem
- IoT
---
