---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: striderintel.com
  spf: true
hosts:
- cert_expires: Sep 18 07:04:04 2026 GMT
  host: www.striderintel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 19:09:21 2026 GMT
  host: app.striderintel.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 19:09:21 2026 GMT
  host: api.striderintel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strider Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strider, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Strider
provider_slug: strider
slug: strider-domain-security
source_filename: strider-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.striderintel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:04:04 2026 GMT\n  hsts: false\n- host: app.striderintel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 19:09:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.striderintel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 19:09:21 2026 GMT\n  hsts: null\ndomains:\n- domain: striderintel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strider/refs/heads/main/security/strider-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Strategic Intelligence
- Threat Intelligence
- Risk Management
- Security
- Supply Chain
- Due Diligence
- Open Source Intelligence
- Artificial Intelligence
- Geopolitical Risk
---
