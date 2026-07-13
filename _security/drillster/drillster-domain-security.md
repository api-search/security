---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: drillster.com
  spf: true
hosts:
- cert_expires: Sep  3 23:59:59 2026 GMT
  host: www.drillster.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drillster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drillster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Drillster
provider_slug: drillster
slug: drillster-domain-security
source_filename: drillster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drillster.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: drillster.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drillster/refs/heads/main/security/drillster-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Assessments
- Education
- Learning
- Quizzes
- Training
- LMS
---
