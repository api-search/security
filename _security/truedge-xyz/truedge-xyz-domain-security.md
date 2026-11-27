---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: true
  domain: truedge.xyz
  spf: true
hosts:
- cert_expires: Feb  9 14:31:06 2027 GMT
  host: truedge.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Truedge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truedge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Truedge
provider_slug: truedge-xyz
slug: truedge-xyz-domain-security
source_filename: truedge-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truedge.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 14:31:06 2027 GMT\n  hsts: false\ndomains:\n- domain: truedge.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/truedge-xyz/security/truedge-xyz-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Crypto
- ScamDetection
- FreeService
- AI
- Education
---
