---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuemail "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "identrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mckesson.com
  spf: true
hosts:
- cert_expires: Aug  8 13:52:39 2026 GMT
  host: www.mckesson.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mckesson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for McKesson, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: McKesson
provider_slug: mckesson
slug: mckesson-domain-security
source_filename: mckesson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mckesson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 13:52:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mckesson.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuemail \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"identrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mckesson/refs/heads/main/security/mckesson-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Distribution
- Fortune 500
- Healthcare
- Medical Supplies
- Pharmaceutical
---
