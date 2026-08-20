---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cafex.ai
  spf: true
- caa:
  - 128 issue "sectigo.com"
  - 128 issuewild "comodoca.com"
  - 128 issuewild "letsencrypt.org"
  - 128 issuewild "sectigo.com"
  - 128 issue "amazonaws.com"
  - 128 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cafex.com
  spf: true
hosts:
- cert_expires: Oct 18 09:09:37 2026 GMT
  host: cafex.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 20:42:14 2026 GMT
  host: support.cafex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 01:53:11 2026 GMT
  host: app.cafex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cafex Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CafeX Communications, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CafeX Communications
provider_slug: cafex-communications
slug: cafex-communications-domain-security
source_filename: cafex-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cafex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 09:09:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.cafex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:42:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.cafex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 01:53:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cafex.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cafex.com\n  dnssec: false\n  caa:\n  - 128 issue \"sectigo.com\"\n  - 128 issuewild \"comodoca.com\"\n  - 128 issuewild \"letsencrypt.org\"\n  - 128 issuewild \"sectigo.com\"\n  - 128 issue \"amazonaws.com\"\n  - 128 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cafex-communications/refs/heads/main/security/cafex-communications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Low-Code
- Workflow-Automation
- Agentic AI
- Audit and Compliance
- Collaboration
- Enterprise Software
- Regulated Industries
- Process Automation
---
