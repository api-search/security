---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: linusbio.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: traced.life
  spf: false
hosts:
- cert_expires: Oct 27 11:30:13 2026 GMT
  host: www.linusbio.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 14:01:01 2026 GMT
  host: traced.life
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linusbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinusBio, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LinusBio
provider_slug: linusbio
slug: linusbio-domain-security
source_filename: linusbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.linusbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 11:30:13 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: traced.life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 14:01:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: linusbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: traced.life\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linusbio/refs/heads/main/security/linusbio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Diagnostics
- Precision Medicine
- Biotechnology
- Exposomics
- Life Sciences
- Autism
- Commerce
- Agents
---
