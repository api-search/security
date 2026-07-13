---
api_specs:
- filename: v1p1
  format: yaml
  label: ClassLink OneRoster API
  slug: classlink-oneroster-api
  spec_type: OpenAPI
  url: https://sandbox-vn-v2.oneroster.com/ims/oneroster/v1p1
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: classlink.com
  spf: true
hosts:
- cert_expires: Sep  9 05:09:33 2026 GMT
  host: www.classlink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 17:10:32 2027 GMT
  host: help.classlink.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: launchpad.classlink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Classlink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClassLink, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClassLink
provider_slug: classlink
slug: classlink-domain-security
source_filename: classlink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.classlink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 05:09:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.classlink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 17:10:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: launchpad.classlink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: classlink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classlink/refs/heads/main/security/classlink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EdTech
- Education
- Identity
- Single Sign-On
- SSO
- OneRoster
- Rostering
- Provisioning
- Analytics
- K-12
- LTI
- OAuth
- Student Data
---
