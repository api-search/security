---
api_specs:
- filename: postman-minis
  format: yaml
  label: Axonius
  slug: axonius
  spec_type: Postman
  url: https://github.com/Axonius/postman-minis
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "axonius.okta.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: axonius.com
  spf: true
hosts:
- cert_expires: Dec  5 20:50:44 2026 GMT
  host: www.axonius.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axonius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axonius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axonius
provider_slug: axonius
slug: axonius-domain-security
source_filename: axonius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axonius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 20:50:44 2026 GMT\n  hsts: null\ndomains:\n- domain: axonius.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"axonius.okta.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axonius/refs/heads/main/security/axonius-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Asset Management
- Cybersecurity
- SaaS Management
- SaaS Security
- Vulnerability Management
- IT Asset Management
- Security Operations
---
