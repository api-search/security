---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: caretaker.com
  spf: true
hosts:
- cert_expires: Oct  8 18:51:36 2026 GMT
  host: caretaker.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caretaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caretaker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Caretaker
provider_slug: caretaker
slug: caretaker-domain-security
source_filename: caretaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caretaker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:51:36 2026 GMT\n  hsts: null\ndomains:\n- domain: caretaker.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caretaker/refs/heads/main/security/caretaker-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
