---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: graco.com
  spf: true
hosts:
- cert_expires: Mar 23 23:59:59 2027 GMT
  host: www.graco.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: developer.graco.com
  https: false
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.graco.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Graco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graco Inc, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Graco Inc
provider_slug: graco
slug: graco-domain-security
source_filename: graco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.graco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.graco.com\n  https: false\n- host: api.graco.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: graco.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graco/refs/heads/main/security/graco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fluid Handling
- Manufacturing
- Industrial
---
