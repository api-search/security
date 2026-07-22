---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: xilis.com
  spf: true
hosts:
- host: xilis.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''xilis.com''.'
kind: domain-security
layout: security
method: probed
name: Xilis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xilis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Xilis
provider_slug: xilis
slug: xilis-domain-security
source_filename: xilis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xilis.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''xilis.com''.'\n  hsts: null\ndomains:\n- domain: xilis.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xilis/refs/heads/main/security/xilis-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Life Sciences
- Precision Oncology
- Biotechnology
- Drug Discovery
- Organoids
---
