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
name: Awake Security Arista Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Awake Security (Arista Networks), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Awake Security (Arista Networks)
provider_slug: awake-security-arista-networks
slug: awake-security-arista-networks-domain-security
source_filename: awake-security-arista-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: awakesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:48:57 2026 GMT\n  hsts: false\ndomains:\n- domain: awakesecurity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awake-security-arista-networks/refs/heads/main/security/awake-security-arista-networks-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Security
- Network Detection and Response
- NDR
- Cybersecurity
- Threat Detection
- Network Security
---
