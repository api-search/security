---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hbfuller.com
  spf: true
hosts:
- cert_expires: Feb 24 18:11:16 2027 GMT
  host: www.hbfuller.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hb Fuller Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for H.B. Fuller, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: H.B. Fuller
provider_slug: hb-fuller
slug: hb-fuller-domain-security
source_filename: hb-fuller-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hbfuller.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 18:11:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hbfuller.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hb-fuller/refs/heads/main/security/hb-fuller-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Adhesives
- Sealants
- Specialty Chemicals
- Industrial
- Manufacturing
- Fortune 1000
---
