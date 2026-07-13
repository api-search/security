---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: htlf.com
  spf: true
hosts:
- host: www.htlf.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.htlf.co'
- host: developer.htlf.com
  https: false
- host: api.htlf.com
  https: false
kind: domain-security
layout: security
method: probed
name: Heartland Financial Usa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heartland Financial USA, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Heartland Financial USA
provider_slug: heartland-financial-usa
slug: heartland-financial-usa-domain-security
source_filename: heartland-financial-usa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.htlf.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.htlf.co'\n  hsts: null\n- host: developer.htlf.com\n  https: false\n- host: api.htlf.com\n  https: false\ndomains:\n- domain: htlf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heartland-financial-usa/refs/heads/main/security/heartland-financial-usa-domain-security.yml
summary_line: DMARC
tags:
- Banking
- Financial Services
---
