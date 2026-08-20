---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cerapedics.com
  spf: true
hosts:
- cert_expires: Oct 22 09:09:47 2026 GMT
  host: www.cerapedics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: mcp.cerapedics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cerapedics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cerapedics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cerapedics
provider_slug: cerapedics
slug: cerapedics-domain-security
source_filename: cerapedics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cerapedics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 09:09:47 2026 GMT\n  hsts: false\n- host: mcp.cerapedics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cerapedics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerapedics/refs/heads/main/security/cerapedics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Orthopedics
- Orthobiologics
- Bone Graft
- Spine Surgery
- Healthcare
- Life Sciences
- MCP
---
