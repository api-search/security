---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: picnic.ai
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: picnichealth.com
  spf: true
hosts:
- cert_expires: Sep 12 22:32:38 2026 GMT
  host: picnic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 20:45:42 2026 GMT
  host: rdocs.picnichealth.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 20:10:32 2026 GMT
  host: rspm.picnichealth.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Picnicai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Picnicai, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Picnicai
provider_slug: picnicai
slug: picnicai-domain-security
source_filename: picnicai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: picnic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 22:32:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rdocs.picnichealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:45:42 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: rspm.picnichealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:10:32 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: picnic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: picnichealth.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picnicai/refs/heads/main/security/picnicai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare Data
- Clinical Research
- Real World Data
- Machine Learning
- Medical Records
- Life Sciences
---
