---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sticky.ai
  spf: true
hosts:
- host: www.sticky.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.sticky.'
kind: domain-security
layout: security
method: probed
name: Sticky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sticky, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sticky
provider_slug: sticky
slug: sticky-domain-security
source_filename: sticky-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sticky.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.sticky.'\n  hsts: null\ndomains:\n- domain: sticky.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sticky/refs/heads/main/security/sticky-domain-security.yml
summary_line: DMARC
tags:
- Company
- Enterprise
- Eye Tracking
- Market Research
- Biometrics
- Emotion Analytics
- Acquired
---
