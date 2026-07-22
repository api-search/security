---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teads.com
  spf: true
- caa:
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:caa@teads.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teads.tv
  spf: true
hosts:
- cert_expires: Sep 16 06:16:14 2026 GMT
  host: www.teads.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 18:02:19 2026 GMT
  host: developers.teads.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:16:14 2026 GMT
  host: ca.teads.tv
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teads Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teads, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Teads
provider_slug: teads
slug: teads-domain-security
source_filename: teads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teads.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:16:14 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developers.teads.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:02:19 2026 GMT\n  hsts: false\n- host: ca.teads.tv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:16:14 2026 GMT\n  hsts: null\ndomains:\n- domain: teads.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: teads.tv\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:caa@teads.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n\
  \  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teads/refs/heads/main/security/teads-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Advertising Technology
- Video Advertising
- Conversions API
- Contextual Advertising
- Mobile SDK
- Conversational AI
---
