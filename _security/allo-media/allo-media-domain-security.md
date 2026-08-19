---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uh.live
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issuewild "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: allo-media.net
  spf: true
hosts:
- cert_expires: Nov 15 09:34:08 2026 GMT
  host: uh.live
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 16:59:19 2026 GMT
  host: docs.allo-media.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 09:34:08 2026 GMT
  host: activate.uh.live
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allo Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allo-Media, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allo-Media
provider_slug: allo-media
slug: allo-media-domain-security
source_filename: allo-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  Probed 2026-08-17. Findings worth reading rather than just recording:\n  TLS 1.3 on all three reachable hosts with valid certs. HSTS is enabled on the\n  marketing host uh.live (max-age 16,000,000 ~ 185 days) but NOT on the API host\n  activate.uh.live or the docs host — the inverse of the priority you would want,\n  since the API host is where bearer tokens travel.\n  The two registrable domains are managed to different standards: allo-media.net\n  has DNSSEC enabled but NO DMARC record, while uh.live has DMARC at p=reject\n  (strong) but no DNSSEC. Each domain has the control the other is missing, which\n  is the signature of a rebrand where DNS hygiene was rebuilt rather than\n  carried across. Both publish SPF and both publish CAA (uh.live pins Let's\n  Encrypt, DigiCert and Comodo; allo-media.net pins the same three including\n  wildcards).\n  Reachability\
  \ caveat: api.uh.live and hermes.allo-media.net could not be probed\n  in this pass because the provider's edge intermittently refuses connections\n  from a single source IP after a short burst; their absence below is our\n  limitation, not a provider defect.\nhosts:\n- host: uh.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 09:34:08 2026 GMT\n  hsts: true\n  hsts_max_age: 16000000\n- host: docs.allo-media.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:59:19 2026 GMT\n  hsts: false\n- host: activate.uh.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 09:34:08 2026 GMT\n  hsts: false\ndomains:\n- domain: uh.live\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: allo-media.net\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  -\
  \ 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allo-media/refs/heads/main/security/allo-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai Data
- Speech Recognition
- Speech To Text
- Conversation Intelligence
- Call Tracking
- Voice AI
- Natural Language Processing
- Call Analytics
- Contact Center
- Speech Analytics
- Transcription
- France
---
