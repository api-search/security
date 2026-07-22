---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spiff.com
  spf: true
hosts:
- host: spiff.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''spiff.com''.'
kind: domain-security
layout: security
method: probed
name: Spiff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spiff, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spiff
provider_slug: spiff
slug: spiff-domain-security
source_filename: spiff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spiff.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''spiff.com''.'\n  hsts: null\ndomains:\n- domain: spiff.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spiff/refs/heads/main/security/spiff-domain-security.yml
summary_line: DMARC
tags:
- Company
- Sales
- Commissions
- Incentive Compensation
- Compensation Management
- Revenue Operations
- Sales Performance
- Acquired
---
