---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lazard.com
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: www.lazard.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: developer.lazard.com
  https: false
- host: api.lazard.com
  https: false
kind: domain-security
layout: security
method: probed
name: Lazard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lazard, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lazard
provider_slug: lazard
slug: lazard-domain-security
source_filename: lazard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lazard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\n- host: developer.lazard.com\n  https: false\n- host: api.lazard.com\n  https: false\ndomains:\n- domain: lazard.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lazard/refs/heads/main/security/lazard-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Investment Banking
- Asset Management
- Financial Advisory
---
