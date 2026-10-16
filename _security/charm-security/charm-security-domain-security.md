---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: charmsecurity.com
  spf: true
hosts:
- cert_expires: Jan  5 12:59:48 2027 GMT
  host: www.charmsecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Charm Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charm Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Charm Security
provider_slug: charm-security
slug: charm-security-domain-security
source_filename: charm-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.charmsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 12:59:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: charmsecurity.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charm-security/refs/heads/main/security/charm-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fraud Prevention
- AI
- Financial Services
- Cybersecurity
- Customer Interaction
---
