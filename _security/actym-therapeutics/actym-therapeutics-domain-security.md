---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: actymthera.com
  spf: true
hosts:
- cert_expires: Oct 22 01:30:12 2026 GMT
  host: www.actymthera.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Actym Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actym Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Actym Therapeutics
provider_slug: actym-therapeutics
slug: actym-therapeutics-domain-security
source_filename: actym-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.actymthera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 01:30:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: actymthera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actym-therapeutics/refs/heads/main/security/actym-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Immuno-Oncology
- Cancer
- Clinical Trials
- Drug Development
- Healthcare
- MCP
---
