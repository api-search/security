---
description: ''
domains:
- caa:
  - 0 issue "twca.com.tw"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qnap.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: qnap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qnap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QNAP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: QNAP
provider_slug: qnap
slug: qnap-domain-security
source_filename: qnap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qnap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qnap.com\n  dnssec: false\n  caa:\n  - 0 issue \"twca.com.tw\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/qnap/security/qnap-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Storage
- NAS
- Enterprise
- Cloud
---
