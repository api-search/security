---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sourcepoint.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 24 06:18:31 2026 GMT
  host: www.sourcepoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:44:01 2026 GMT
  host: docs.sourcepoint.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: sourcepoint-public-api.readme.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sourcepoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sourcepoint, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sourcepoint
provider_slug: sourcepoint
slug: sourcepoint-domain-security
source_filename: sourcepoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sourcepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 06:18:31 2026 GMT\n  hsts: false\n- host: docs.sourcepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:44:01 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: sourcepoint-public-api.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: null\ndomains:\n- domain: sourcepoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sourcepoint/refs/heads/main/security/sourcepoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Privacy
- Consent Management
- Consent Management Platform
- CMP
- GDPR
- CCPA
- LGPD
- IAB TCF
- IAB GPP
- USNAT
- DSAR
- Adblock Recovery
- Compliance Monitoring
- Publisher Technology
- AdTech
- MarTech
- Privacy Engineering
- CTV
- OTT
- Mobile SDK
- Web SDK
---
