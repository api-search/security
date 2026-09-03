---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: enigma-health.org
  spf: true
hosts:
- cert_expires: Nov  4 04:49:51 2026 GMT
  host: enigma-health.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Enigma Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enigma Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Enigma Health
provider_slug: enigma-health
slug: enigma-health-domain-security
source_filename: enigma-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enigma-health.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 04:49:51 2026 GMT\n  hsts: false\ndomains:\n- domain: enigma-health.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enigma-health/refs/heads/main/security/enigma-health-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Health
- Healthcare
- Electronic Health Records
- openEHR
- Digital Health
- Interoperability
- Patient Data
- Netherlands
- Startup
---
