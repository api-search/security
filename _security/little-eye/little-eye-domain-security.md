---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: littleeye.co
  spf: true
hosts:
- cert_expires: Oct 15 21:00:55 2026 GMT
  host: littleeye.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Little Eye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Little Eye, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Little Eye
provider_slug: little-eye
slug: little-eye-domain-security
source_filename: little-eye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: littleeye.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:00:55 2026 GMT\n  hsts: false\ndomains:\n- domain: littleeye.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/little-eye/refs/heads/main/security/little-eye-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Blog
- Technology News
- Defunct
---
