---
description: ''
domains:
- caa:
  - 0 iodef "mailto:hostmaster@scb.se"
  - 0 issue "expisoft.se"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scb.se
  spf: true
hosts:
- cert_expires: Dec 23 07:24:57 2026 GMT
  host: scb.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SCB Statistics Sweden, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SCB Statistics Sweden
provider_slug: scb
slug: scb-domain-security
source_filename: scb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scb.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 07:24:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scb.se\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:hostmaster@scb.se\"\n  - 0 issue \"expisoft.se\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scb/refs/heads/main/security/scb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Statistics
- Sweden
- Government
- Data
---
