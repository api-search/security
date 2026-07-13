---
api_specs:
- filename: djangocms-rest-openapi.yml
  format: yaml
  label: djangocms-rest API
  slug: djangocms-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/django-cms/main/openapi/djangocms-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: django-cms.org
  spf: true
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Sep 19 14:02:44 2026 GMT
  host: www.django-cms.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: djangocms-rest.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Django Cms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Django CMS, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Django CMS
provider_slug: django-cms
slug: django-cms-domain-security
source_filename: django-cms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.django-cms.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 14:02:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: djangocms-rest.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: django-cms.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/django-cms/refs/heads/main/security/django-cms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Management
- Django
- Python
- Headless CMS
- REST API
- Open Source
- Pages
- Plugins
- Placeholders
---
