---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: useretainer.com
  spf: true
hosts:
- cert_expires: Feb 14 20:21:50 2027 GMT
  host: useretainer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Useretainer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Useretainer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Useretainer
provider_slug: useretainer-com
slug: useretainer-com-domain-security
source_filename: useretainer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: useretainer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 20:21:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: useretainer.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/useretainer-com/security/useretainer-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- CRM
- Consulting
- SaaS
- Retainer
- Productivity
---
