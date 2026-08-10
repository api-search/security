---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: recurohealth.com
  spf: true
hosts:
- cert_expires: Oct 22 01:36:25 2026 GMT
  host: recurohealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 09:14:02 2026 GMT
  host: auth.recurohealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recuro Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recuro Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Recuro Health
provider_slug: recuro-health
slug: recuro-health-domain-security
source_filename: recuro-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recurohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 01:36:25 2026 GMT\n  hsts: false\n- host: auth.recurohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 09:14:02 2026 GMT\n  hsts: false\ndomains:\n- domain: recurohealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recuro-health/refs/heads/main/security/recuro-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- Telehealth
- Virtual Care
- Digital Health
- Behavioral Health
- Primary Care
- Employee Benefits
- Health Plans
- Identity
- OpenID Connect
---
