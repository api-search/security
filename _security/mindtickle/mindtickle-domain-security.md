---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mindtickle.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.mindtickle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: api.mindtickle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api-gateway.callai.www.mindtickle.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''api-gateway'
kind: domain-security
layout: security
method: probed
name: Mindtickle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mindtickle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mindtickle
provider_slug: mindtickle
slug: mindtickle-domain-security
source_filename: mindtickle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mindtickle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mindtickle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\n- host: api-gateway.callai.www.mindtickle.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''api-gateway'\n  hsts: null\ndomains:\n- domain: mindtickle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindtickle/refs/heads/main/security/mindtickle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Enablement
- Revenue Productivity
- Sales Readiness
- Coaching
- Conversation Intelligence
- Learning Management
- Content Management
- Call AI
- Revenue Intelligence
---
