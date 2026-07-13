---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "dtrust.de"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issue "microsoft.com"
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: office.com
  spf: false
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec  7 02:00:39 2026 GMT
  host: forms.office.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Forms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Forms, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: Microsoft Forms
provider_slug: microsoft-forms
slug: microsoft-forms-domain-security
source_filename: microsoft-forms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forms.office.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 02:00:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: office.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"dtrust.de\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"microsoft.com\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-forms/refs/heads/main/security/microsoft-forms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Forms
- Microsoft
- Microsoft 365
- Quizzes
- Surveys
---
