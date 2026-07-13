---
description: ''
domains:
- caa:
  - 0 issue "rapidssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cloudbees.com
  spf: true
hosts:
- cert_expires: Sep 24 07:28:40 2026 GMT
  host: docs.cloudbees.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codeship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codeship, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Codeship
provider_slug: codeship
slug: codeship-domain-security
source_filename: codeship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.cloudbees.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 07:28:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudbees.com\n  dnssec: false\n  caa:\n  - 0 issue \"rapidssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codeship/refs/heads/main/security/codeship-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Continuous Integration
- Public APIs
---
