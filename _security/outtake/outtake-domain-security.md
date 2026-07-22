---
description: ''
domains:
- caa:
  - 0 iodef "mailto:hello@outtake.ai"
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: outtake.ai
  spf: true
hosts:
- cert_expires: Oct 14 13:59:41 2026 GMT
  host: outtake.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outtake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outtake, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Outtake
provider_slug: outtake
slug: outtake-domain-security
source_filename: outtake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outtake.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 13:59:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: outtake.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:hello@outtake.ai\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outtake/refs/heads/main/security/outtake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Digital Risk Protection
- Threat Intelligence
- Brand Protection
- Anti-Fraud
- Artificial Intelligence
- Takedown
---
