---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tigereye.com
  spf: true
hosts:
- cert_expires: Sep 11 18:03:32 2026 GMT
  host: tigereye.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tigereye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TigerEye, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TigerEye
provider_slug: tigereye
slug: tigereye-domain-security
source_filename: tigereye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tigereye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:03:32 2026 GMT\n  hsts: false\ndomains:\n- domain: tigereye.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigereye/refs/heads/main/security/tigereye-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Construction
- Construction Technology
- Business Intelligence
- Enterprise Saas
---
