---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: karat.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slab.com
  spf: true
hosts:
- cert_expires: Sep 22 03:42:08 2026 GMT
  host: karat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:45:25 2026 GMT
  host: karat.slab.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karat, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Karat
provider_slug: karat
slug: karat-domain-security
source_filename: karat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: karat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:42:08 2026 GMT\n  hsts: null\n- host: karat.slab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:45:25 2026 GMT\n  hsts: null\ndomains:\n- domain: karat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: slab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karat/refs/heads/main/security/karat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technical Interviewing
- Hiring
- Recruiting
- Talent Assessment
- Engineering
- GraphQL
- API
---
