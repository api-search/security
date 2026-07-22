---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: headway.co
  spf: true
hosts:
- cert_expires: Oct 11 00:15:47 2026 GMT
  host: headway.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Headway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Headway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Headway
provider_slug: headway
slug: headway-domain-security
source_filename: headway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: headway.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 00:15:47 2026 GMT\n  hsts: null\ndomains:\n- domain: headway.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/headway/refs/heads/main/security/headway-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mental Health
- Healthcare
- Behavioral Health
- Therapy
- Insurance
- Health Tech
---
