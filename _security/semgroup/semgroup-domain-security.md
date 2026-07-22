---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: semgroup.com
  spf: true
hosts:
- host: www.semgroup.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.semgrou'
kind: domain-security
layout: security
method: probed
name: Semgroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for semgroup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: semgroup
provider_slug: semgroup
slug: semgroup-domain-security
source_filename: semgroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.semgroup.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.semgrou'\n  hsts: null\ndomains:\n- domain: semgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semgroup/refs/heads/main/security/semgroup-domain-security.yml
summary_line: DMARC
tags:
- Fortune 1000
---
