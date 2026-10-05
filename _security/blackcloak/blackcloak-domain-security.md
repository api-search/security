---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: blackcloak.io
  spf: true
hosts:
- cert_expires: Nov 11 05:54:28 2026 GMT
  host: blackcloak.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blackcloak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blackcloak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Blackcloak
provider_slug: blackcloak
slug: blackcloak-domain-security
source_filename: blackcloak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blackcloak.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 05:54:28 2026 GMT\n  hsts: null\ndomains:\n- domain: blackcloak.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackcloak/refs/heads/main/security/blackcloak-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Security
- Cybersecurity
- Executive Protection
- PersonalSafety
- Digital Identity
---
