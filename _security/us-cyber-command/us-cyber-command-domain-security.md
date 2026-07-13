---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cybercom.mil
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: virustotal.com
  spf: true
hosts:
- cert_expires: Aug 17 15:25:38 2026 GMT
  host: www.cybercom.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 03:26:46 2026 GMT
  host: www.virustotal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Cyber Command Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Cyber Command, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Cyber Command
provider_slug: us-cyber-command
slug: us-cyber-command-domain-security
source_filename: us-cyber-command-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cybercom.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:25:38 2026 GMT\n  hsts: null\n- host: www.virustotal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:26:46 2026 GMT\n  hsts: null\ndomains:\n- domain: cybercom.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: virustotal.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-cyber-command/refs/heads/main/security/us-cyber-command-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cybersecurity
- Federal Government
- Military
- Threat Intelligence
- Defense
---
