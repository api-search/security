---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kennasecurity.com
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.kennasecurity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:38:45 2026 GMT
  host: apidocs.kennasecurity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: api.kennasecurity.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kenna Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kenna Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kenna Security
provider_slug: kenna-security
slug: kenna-security-domain-security
source_filename: kenna-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kennasecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\n- host: apidocs.kennasecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:38:45 2026 GMT\n  hsts: null\n- host: api.kennasecurity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kennasecurity.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kenna-security/refs/heads/main/security/kenna-security-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cybersecurity
- Vulnerability Management
- Risk-Based Prioritization
- Threat Intelligence
- Security
- Cisco
- REST API
---
