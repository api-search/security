---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usercentrics.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vero-ai.com
  spf: true
hosts:
- cert_expires: Sep 15 05:37:49 2026 GMT
  host: usercentrics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 07:56:57 2026 GMT
  host: www.vero-ai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 14:18:53 2026 GMT
  host: riskonnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regulatory Templates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regulatory Templates, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Regulatory Templates
provider_slug: regulatory-templates
slug: regulatory-templates-domain-security
source_filename: regulatory-templates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usercentrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:37:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.vero-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 07:56:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: riskonnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 14:18:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usercentrics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vero-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regulatory-templates/refs/heads/main/security/regulatory-templates-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Governance
- GDPR
- HIPAA
- ISO 27001
- PCI DSS
- Policy Templates
- Regulatory
- SOC 2
- Templates
---
