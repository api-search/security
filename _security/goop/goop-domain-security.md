---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goop.com
  spf: true
hosts:
- cert_expires: Oct 14 18:56:16 2026 GMT
  host: goop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Goop
provider_slug: goop
slug: goop-domain-security
source_filename: goop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:56:16 2026 GMT\n  hsts: null\ndomains:\n- domain: goop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goop/refs/heads/main/security/goop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wellness
- Lifestyle
- Beauty
- E-Commerce
- Content
- Health
- Consumer Brand
- Retail
---
