---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: isa.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opcfoundation.org
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.isa.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 01:15:05 2026 GMT
  host: opcfoundation.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 20:15:21 2026 GMT
  host: mqtt.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SCADA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SCADA
provider_slug: scada
slug: scada-domain-security
source_filename: scada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.isa.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: opcfoundation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:15:05 2026 GMT\n  hsts: false\n- host: mqtt.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 20:15:21 2026 GMT\n  hsts: false\ndomains:\n- domain: isa.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: opcfoundation.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scada/refs/heads/main/security/scada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Critical Infrastructure
- ICS
- Industrial Automation
- Industrial IoT
- OT Security
- SCADA
---
