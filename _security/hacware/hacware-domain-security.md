---
api_specs:
- filename: hacware-openapi.yml
  format: yaml
  label: HacWare Security Awareness API
  slug: hacware-security-awareness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/openapi/hacware-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hacware.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: hacware.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.hacware.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: app.hacware.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hacware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hacware, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hacware
provider_slug: hacware
slug: hacware-domain-security
source_filename: hacware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hacware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: www.hacware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: app.hacware.com\n  https: false\ndomains:\n- domain: hacware.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hacware/refs/heads/main/security/hacware-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Security
- Cybersecurity
- Security Awareness
- Phishing
- Training
- Compliance
- Email Security
- Artificial Intelligence
---
