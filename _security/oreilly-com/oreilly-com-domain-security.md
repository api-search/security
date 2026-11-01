---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 iodef "mailto:itops@oreilly.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oreilly.com
  spf: true
hosts:
- cert_expires: Jan 15 23:09:20 2027 GMT
  host: oreilly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oreilly Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for oreilly-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: oreilly-com
provider_slug: oreilly-com
slug: oreilly-com-domain-security
source_filename: oreilly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oreilly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:09:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oreilly.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:itops@oreilly.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oreilly-com/security/oreilly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Technology
- Training
- Publishing
---
