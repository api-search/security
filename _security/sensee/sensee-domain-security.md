---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sensee.com
  spf: true
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: sensee.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sensee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sensee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sensee
provider_slug: sensee
slug: sensee-domain-security
source_filename: sensee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sensee.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sensee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensee/refs/heads/main/security/sensee-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Consumer
- Eyewear
- Contact Lenses
- Optical
- E-Commerce
- Healthcare
- Retail
- Europe
---
