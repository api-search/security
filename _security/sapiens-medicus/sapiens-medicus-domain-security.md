---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: esculap.io
  spf: false
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: esculap.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sapiens Medicus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sapiens Medicus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Sapiens Medicus
provider_slug: sapiens-medicus
slug: sapiens-medicus-domain-security
source_filename: sapiens-medicus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: esculap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: esculap.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sapiens-medicus/refs/heads/main/security/sapiens-medicus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health
- Artificial Intelligence
- Medical
- Telehealth
- Consumer Health
- Diagnostics
---
