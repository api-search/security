---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: robustintelligence.com
  spf: false
- caa:
  - 0 issue "globalsign.com"
  - 128 issuewild "identrust.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 128 iodef "mailto:infosec@cisco.com"
  - 128 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cisco.com
  spf: true
hosts:
- host: www.robustintelligence.com
  https: false
- cert_expires: Nov  9 01:46:22 2026 GMT
  host: www.cisco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Robust Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Robust Intelligence, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Robust Intelligence
provider_slug: robust-intelligence
slug: robust-intelligence-domain-security
source_filename: robust-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.robustintelligence.com\n  https: false\n- host: www.cisco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 01:46:22 2026 GMT\n  hsts: null\ndomains:\n- domain: robustintelligence.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: cisco.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 128 issuewild \"identrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 128 iodef \"mailto:infosec@cisco.com\"\n  - 128 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robust-intelligence/refs/heads/main/security/robust-intelligence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Security
- Runtime Protection
- Algorithmic Red Teaming
- LLM Security
- Cisco
- Acquired
- Guardrails
---
