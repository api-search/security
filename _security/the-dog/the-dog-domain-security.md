---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: thedogapi.com
  spf: true
hosts:
- cert_expires: Oct  5 18:10:00 2026 GMT
  host: thedogapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Dog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Dog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: The Dog
provider_slug: the-dog
slug: the-dog-domain-security
source_filename: the-dog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thedogapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:10:00 2026 GMT\n  hsts: false\ndomains:\n- domain: thedogapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-dog/refs/heads/main/security/the-dog-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Animals
- Public APIs
---
