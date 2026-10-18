---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jukshio.com
  spf: true
hosts:
- cert_expires: Jan  5 19:05:10 2027 GMT
  host: jukshio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jukshio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jukshio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Jukshio
provider_slug: jukshio
slug: jukshio-domain-security
source_filename: jukshio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jukshio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:05:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jukshio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jukshio/refs/heads/main/security/jukshio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- IdentityVerification
- KYC
- Enterprise
---
