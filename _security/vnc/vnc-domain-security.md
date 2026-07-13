---
api_specs:
- filename: vnc-cloud-openapi.yml
  format: yaml
  label: VNC Cloud API
  slug: vnc-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vnc/refs/heads/main/openapi/vnc-cloud-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "symantec.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: realvnc.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vnc.com
  spf: true
hosts:
- cert_expires: Aug 25 21:56:28 2026 GMT
  host: www.realvnc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.vnc.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vnc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VNC, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VNC
provider_slug: vnc
slug: vnc-domain-security
source_filename: vnc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.realvnc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 21:56:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.vnc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: realvnc.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"symantec.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vnc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vnc/refs/heads/main/security/vnc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Remote Desktop
- Remote Access
- VNC
- Networking
- Screen Sharing
---
