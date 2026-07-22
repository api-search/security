---
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issue "amazon.com"
  - 128 issue "godaddy.com"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onemedical.com
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: onemedical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: One Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for One Medical *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: One Medical *
provider_slug: one-medical
slug: one-medical-domain-security
source_filename: one-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onemedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onemedical.com\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"amazon.com\"\n  - 128 issue \"godaddy.com\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-medical/refs/heads/main/security/one-medical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Healthcare
- Primary Care
- Telehealth
- Amazon
---
