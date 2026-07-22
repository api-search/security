---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: insperity.com
  spf: true
hosts:
- cert_expires: Nov 24 14:08:01 2026 GMT
  host: www.insperity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insperity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for insperity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: insperity
provider_slug: insperity
slug: insperity-domain-security
source_filename: insperity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.insperity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 14:08:01 2026 GMT\n  hsts: null\ndomains:\n- domain: insperity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insperity/refs/heads/main/security/insperity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 1000
---
