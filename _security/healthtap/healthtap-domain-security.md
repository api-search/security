---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:devops+caa@healthtap.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: healthtap.com
  spf: true
hosts:
- cert_expires: Feb  3 17:41:12 2027 GMT
  host: www.healthtap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healthtap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HealthTap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HealthTap
provider_slug: healthtap
slug: healthtap-domain-security
source_filename: healthtap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.healthtap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 17:41:12 2027 GMT\n  hsts: null\ndomains:\n- domain: healthtap.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:devops+caa@healthtap.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthtap/refs/heads/main/security/healthtap-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health Tech
- Telehealth
- Telemedicine
- Virtual Care
- Healthcare
- Primary Care
- Digital Health
---
