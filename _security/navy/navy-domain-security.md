---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: navy.mil
  spf: true
hosts:
- cert_expires: Sep 27 17:48:31 2026 GMT
  host: www.navy.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 20 12:07:20 2026 GMT
  host: www.cnatra.navy.mil
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Navy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Navy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Navy
provider_slug: navy
slug: navy-domain-security
source_filename: navy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.navy.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:48:31 2026 GMT\n  hsts: null\n- host: www.cnatra.navy.mil\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 20 12:07:20 2026 GMT\n  hsts: null\ndomains:\n- domain: navy.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navy/refs/heads/main/security/navy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Military
- Defense
---
