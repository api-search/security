---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:cybersecurity@saronic.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saronic.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.saronic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saronic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saronic Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Saronic Technologies
provider_slug: saronic
slug: saronic-domain-security
source_filename: saronic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saronic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: saronic.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:cybersecurity@saronic.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saronic/refs/heads/main/security/saronic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Defense
- Maritime
- Autonomous Surface Vessels
- ASV
- Echelon
- Command and Control
- Mission Software
- Unmanned Systems
- ITAR
- Naval
---
