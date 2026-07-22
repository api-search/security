---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: avient.com
  spf: true
hosts:
- cert_expires: Aug 13 05:44:57 2026 GMT
  host: www.avient.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polyone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for polyone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: polyone
provider_slug: polyone
slug: polyone-domain-security
source_filename: polyone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avient.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 05:44:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: avient.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polyone/refs/heads/main/security/polyone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
