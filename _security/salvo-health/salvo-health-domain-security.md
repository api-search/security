---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: salvohealth.com
  spf: false
hosts:
- cert_expires: Sep 27 21:19:09 2026 GMT
  host: www.salvohealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salvo Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salvo Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Salvo Health
provider_slug: salvo-health
slug: salvo-health-domain-security
source_filename: salvo-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.salvohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:19:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: salvohealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salvo-health/refs/heads/main/security/salvo-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Gastrointestinal
- Metabolic Health
- Remote Patient Monitoring
- Virtual Care
- EHR Integration
---
