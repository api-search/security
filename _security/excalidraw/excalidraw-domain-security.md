---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: excalidraw.com
  spf: true
hosts:
- cert_expires: Aug 18 06:55:03 2026 GMT
  host: excalidraw.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 11:13:30 2026 GMT
  host: docs.excalidraw.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Excalidraw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Excalidraw, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Excalidraw
provider_slug: excalidraw
slug: excalidraw-domain-security
source_filename: excalidraw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: excalidraw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 06:55:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.excalidraw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 11:13:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: excalidraw.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/excalidraw/refs/heads/main/security/excalidraw-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Whiteboard
- Diagramming
- Open Source
- Drawing
---
