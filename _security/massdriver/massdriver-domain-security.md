---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@massdriver.cloud"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: massdriver.cloud
  spf: true
hosts:
- cert_expires: Sep 26 13:28:10 2026 GMT
  host: www.massdriver.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Massdriver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Massdriver, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Massdriver
provider_slug: massdriver
slug: massdriver-domain-security
source_filename: massdriver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.massdriver.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:28:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: massdriver.cloud\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@massdriver.cloud\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/massdriver/refs/heads/main/security/massdriver-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Infrastructure
- Developer Experience
- Internal Developer Platform
---
