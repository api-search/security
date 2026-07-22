---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: awakesecurity.com
  spf: true
hosts:
- cert_expires: Oct  8 19:48:57 2026 GMT
  host: awakesecurity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Awake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Awake, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Awake
provider_slug: awake
slug: awake-domain-security
source_filename: awake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: awakesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:48:57 2026 GMT\n  hsts: false\ndomains:\n- domain: awakesecurity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awake/refs/heads/main/security/awake-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Network Detection and Response
- Network Security
- Threat Detection
- Security Analytics
- Greylock Portfolio
---
