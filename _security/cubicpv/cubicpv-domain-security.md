---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cubicpv.com
  spf: true
hosts:
- cert_expires: Dec 18 16:17:45 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 09:41:35 2026 GMT
  host: cubicpv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Cubicpv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CubicPV, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CubicPV
provider_slug: cubicpv
slug: cubicpv-domain-security
source_filename: cubicpv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 16:17:45 2026 GMT\n  hsts: null\n- host: cubicpv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 09:41:35 2026 GMT\n  hsts: false\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cubicpv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubicpv/refs/heads/main/security/cubicpv-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductors
- Perovskite
- Solar
- Innovation
---
