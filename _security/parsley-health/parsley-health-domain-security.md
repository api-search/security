---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parsleyhealth.com
  spf: true
hosts:
- cert_expires: Oct  3 22:23:12 2026 GMT
  host: www.parsleyhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 04:18:48 2026 GMT
  host: my.parsleyhealth.com
  hsts: false
  https: true
  note: authenticated member application (Google Frontend); no HSTS response header observed
  tls_version: TLSv1.3
- cert_expires: Sep 18 21:14:35 2026 GMT
  host: app.parsleyhealth.com
  hsts: false
  https: true
  note: authenticated member application (Google Frontend); no HSTS response header observed
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parsley Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parsley Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Parsley Health
provider_slug: parsley-health
slug: parsley-health-domain-security
source_filename: parsley-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parsleyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:23:12 2026 GMT\n  hsts: false\n- host: my.parsleyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:18:48 2026 GMT\n  hsts: false\n  note: authenticated member application (Google Frontend); no HSTS response header observed\n- host: app.parsleyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:14:35 2026 GMT\n  hsts: false\n  note: authenticated member application (Google Frontend); no HSTS response header observed\ndomains:\n- domain: parsleyhealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsley-health/refs/heads/main/security/parsley-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- Telehealth
- Telemedicine
- Functional Medicine
- Primary Care
- Wellness
- Nutrition
- Diagnostics
- Lab Testing
- Membership
- Digital Health
- Consumer Health
---
