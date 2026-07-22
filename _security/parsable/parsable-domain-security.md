---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parsable.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: parsable.net
  spf: false
hosts:
- cert_expires: Sep 25 14:31:28 2026 GMT
  host: parsable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: apidocs.parsable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: api.parsable.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parsable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parsable, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Parsable
provider_slug: parsable
slug: parsable-domain-security
source_filename: parsable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parsable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:31:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.parsable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\n- host: api.parsable.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: parsable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: parsable.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsable/refs/heads/main/security/parsable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Connected Worker
- Manufacturing
- Industrial
- Digital Work Instructions
- Frontline Operations
- Workflow
- Analytics
---
