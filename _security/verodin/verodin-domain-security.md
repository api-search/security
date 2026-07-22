---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "awstrust.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verodin.com
  spf: true
hosts:
- cert_expires: Aug  5 20:17:52 2026 GMT
  host: www.verodin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verodin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verodin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verodin
provider_slug: verodin
slug: verodin-domain-security
source_filename: verodin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verodin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 20:17:52 2026 GMT\n  hsts: null\ndomains:\n- domain: verodin.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verodin/refs/heads/main/security/verodin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cybersecurity
- Security Validation
- Breach and Attack Simulation
- Security Instrumentation
- Acquired
- Mandiant
---
