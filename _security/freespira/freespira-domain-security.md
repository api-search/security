---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: freespira.com
  spf: true
hosts:
- cert_expires: Sep  2 09:04:20 2026 GMT
  host: freespira.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freespira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freespira, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Freespira
provider_slug: freespira
slug: freespira-domain-security
source_filename: freespira-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freespira.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 09:04:20 2026 GMT\n  hsts: false\ndomains:\n- domain: freespira.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freespira/refs/heads/main/security/freespira-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Therapeutics
- Mental Health
- Medical Device
- PTSD
- Anxiety
---
