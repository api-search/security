---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: actions-semi.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.actions-semi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Actions Semiconductor Co Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actions Semiconductor Co., Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Actions Semiconductor Co., Ltd.
provider_slug: actions-semiconductor-co-ltd
slug: actions-semiconductor-co-ltd-domain-security
source_filename: actions-semiconductor-co-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.actions-semi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: actions-semi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/actions-semiconductor-co-ltd/security/actions-semiconductor-co-ltd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductor
- AI
- Edge Computing
- Low Power
- IoT
---
