---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01"
  - 0 issue "amazonaws.com"
  - 0 issue "certainly.com;validationmethods=dns-01"
  dmarc: false
  dnssec: false
  domain: djangoproject.com
  spf: true
hosts:
- cert_expires: Sep 26 08:21:15 2026 GMT
  host: www.djangoproject.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Django Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Django, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Django
provider_slug: django
slug: django-domain-security
source_filename: django-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.djangoproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:21:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: djangoproject.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"certainly.com;validationmethods=dns-01\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/django/refs/heads/main/security/django-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Backend
- MVC
- ORM
- Python
- Web Framework
---
