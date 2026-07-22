---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zenbusiness.com
  spf: true
hosts:
- cert_expires: Sep 22 03:33:03 2026 GMT
  host: www.zenbusiness.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenbusiness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZenBusiness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ZenBusiness
provider_slug: zenbusiness
slug: zenbusiness-domain-security
source_filename: zenbusiness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zenbusiness.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:33:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: zenbusiness.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenbusiness/refs/heads/main/security/zenbusiness-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Business Formation
- LLC Formation
- Registered Agent
- Compliance
- SMB
- Legal Tech
---
