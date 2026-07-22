---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: safetywing.com
  spf: true
hosts:
- cert_expires: Sep 18 07:07:54 2026 GMT
  host: safetywing.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Safety Wing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Safety Wing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Safety Wing
provider_slug: safety-wing
slug: safety-wing-domain-security
source_filename: safety-wing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: safetywing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:07:54 2026 GMT\n  hsts: false\ndomains:\n- domain: safetywing.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safety-wing/refs/heads/main/security/safety-wing-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Insurance
- Insurtech
- Travel Insurance
- Health Insurance
- Remote Work
- Digital Nomads
---
