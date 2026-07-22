---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: africom.mil
  spf: false
hosts:
- cert_expires: Nov 18 19:54:40 2026 GMT
  host: www.africom.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United States Africa Command Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United States Africa Command, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: United States Africa Command
provider_slug: united-states-africa-command
slug: united-states-africa-command-domain-security
source_filename: united-states-africa-command-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.africom.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 19:54:40 2026 GMT\n  hsts: null\ndomains:\n- domain: africom.mil\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-africa-command/refs/heads/main/security/united-states-africa-command-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Military
- Defense
- Africa
---
