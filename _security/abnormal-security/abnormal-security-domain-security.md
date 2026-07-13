---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abnormal.ai
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abnormalsecurity.com
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: abnormal.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: portal.abnormalsecurity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 00:01:41 2026 GMT
  host: api.abnormalplatform.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abnormal Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abnormal Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Abnormal Security
provider_slug: abnormal-security
slug: abnormal-security-domain-security
source_filename: abnormal-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abnormal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.abnormalsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\n- host: api.abnormalplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:01:41 2026 GMT\n  hsts: null\ndomains:\n- domain: abnormal.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: abnormalsecurity.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abnormal-security/refs/heads/main/security/abnormal-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- Email Security
- Account Takeover
- Behavioral AI
- SaaS Security
- Phishing
- BEC
---
