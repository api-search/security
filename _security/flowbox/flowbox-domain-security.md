---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getflowbox.com
  spf: true
hosts:
- cert_expires: Dec 10 03:01:15 2026 GMT
  host: getflowbox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flowbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flowbox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flowbox
provider_slug: flowbox
slug: flowbox-domain-security
source_filename: flowbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getflowbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 03:01:15 2026 GMT\n  hsts: null\ndomains:\n- domain: getflowbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowbox/refs/heads/main/security/flowbox-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
