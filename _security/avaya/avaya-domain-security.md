---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avaya.com
  spf: true
hosts:
- cert_expires: Sep 25 21:49:27 2026 GMT
  host: www.avaya.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: developers.avaya.com
  https: false
kind: domain-security
layout: security
method: probed
name: Avaya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avaya, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avaya
provider_slug: avaya
slug: avaya-domain-security
source_filename: avaya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avaya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 21:49:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developers.avaya.com\n  https: false\ndomains:\n- domain: avaya.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avaya/refs/heads/main/security/avaya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- Contact Center
- Collaboration
- AI
- UCaaS
---
