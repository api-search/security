---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:cory.watson@chainalysis.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chainalysis.com
  spf: true
hosts:
- cert_expires: Nov 21 13:04:02 2026 GMT
  host: www.chainalysis.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chainalysis123 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chainalysis123, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chainalysis123
provider_slug: chainalysis123
slug: chainalysis123-domain-security
source_filename: chainalysis123-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chainalysis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 13:04:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: chainalysis.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:cory.watson@chainalysis.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainalysis123/refs/heads/main/security/chainalysis123-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- blockchain analytics
- crypto compliance
- investigations
- financial institutions
- law enforcement
- Exchange
- Security
- data solutions
---
