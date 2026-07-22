---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cruxocm.com
  spf: true
hosts:
- cert_expires: Sep 27 16:54:36 2026 GMT
  host: cruxocm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crux Ocm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crux OCM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crux OCM
provider_slug: crux-ocm
slug: crux-ocm-domain-security
source_filename: crux-ocm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cruxocm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:54:36 2026 GMT\n  hsts: false\ndomains:\n- domain: cruxocm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crux-ocm/refs/heads/main/security/crux-ocm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Industrial Automation
- Pipeline Operations
- Energy
- SCADA
- Control Systems
- Midstream
- Industrial Control
---
