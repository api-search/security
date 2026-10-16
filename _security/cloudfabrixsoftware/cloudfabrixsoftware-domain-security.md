---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fabrix.ai
  spf: true
hosts:
- cert_expires: Jan  7 01:54:34 2027 GMT
  host: fabrix.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloudfabrixsoftware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudfabrixsoftware, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cloudfabrixsoftware
provider_slug: cloudfabrixsoftware
slug: cloudfabrixsoftware-domain-security
source_filename: cloudfabrixsoftware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fabrix.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 01:54:34 2027 GMT\n  hsts: false\ndomains:\n- domain: fabrix.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudfabrixsoftware/refs/heads/main/security/cloudfabrixsoftware-domain-security.yml
summary_line: TLSv1.2
tags:
- AI
- Platform
- Enterprise
- Automation
- Cloud
---
