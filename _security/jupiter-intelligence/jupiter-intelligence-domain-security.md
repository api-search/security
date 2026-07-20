---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jupiterintel.com
  spf: true
hosts:
- cert_expires: Sep 28 08:11:04 2026 GMT
  host: www.jupiterintel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.jupiterintel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jupiter Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jupiter Intelligence, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jupiter Intelligence
provider_slug: jupiter-intelligence
slug: jupiter-intelligence-domain-security
source_filename: jupiter-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jupiterintel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:11:04 2026 GMT\n  hsts: null\n- host: api.jupiterintel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jupiterintel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupiter-intelligence/refs/heads/main/security/jupiter-intelligence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate Risk
- Physical Risk Analytics
- Climate Data
- Weather Risk
- Financial Risk
- ESG
- Analytics
---
