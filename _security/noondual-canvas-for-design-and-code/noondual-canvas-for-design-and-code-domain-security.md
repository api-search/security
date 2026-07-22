---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:dmarc-reports@noon.design"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: noon.design
  spf: true
hosts:
- cert_expires: Sep  3 12:48:29 2026 GMT
  host: noon.design
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noondual Canvas For Design And Code Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noondual-canvas for design and code, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Noondual-canvas for design and code
provider_slug: noondual-canvas-for-design-and-code
slug: noondual-canvas-for-design-and-code-domain-security
source_filename: noondual-canvas-for-design-and-code-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noon.design\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 12:48:29 2026 GMT\n  hsts: null\ndomains:\n- domain: noon.design\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:dmarc-reports@noon.design\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noondual-canvas-for-design-and-code/refs/heads/main/security/noondual-canvas-for-design-and-code-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Developer Tools
- Design
- Design Tools
- Code
---
