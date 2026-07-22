---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quidelortho.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: myquidel.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.quidelortho.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.myquidel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quidelortho Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuidelOrtho, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: QuidelOrtho
provider_slug: quidelortho
slug: quidelortho-domain-security
source_filename: quidelortho-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quidelortho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.myquidel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: quidelortho.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: myquidel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quidelortho/refs/heads/main/security/quidelortho-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Diagnostics
- Healthcare
- Medical Devices
- In Vitro Diagnostics
- Laboratory
---
