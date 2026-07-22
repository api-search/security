---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:caa-audit@bluevoyant.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bluevoyant.com
  spf: true
hosts:
- cert_expires: Oct  6 22:17:16 2026 GMT
  host: bluevoyant.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluevoyant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluevoyant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bluevoyant
provider_slug: bluevoyant
slug: bluevoyant-domain-security
source_filename: bluevoyant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluevoyant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:16 2026 GMT\n  hsts: null\ndomains:\n- domain: bluevoyant.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:caa-audit@bluevoyant.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluevoyant/refs/heads/main/security/bluevoyant-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Managed Detection and Response
- Threat Intelligence
- Supply Chain Security
- Digital Risk Protection
- Security Operations
---
