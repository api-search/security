---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: enzo.com
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.enzo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enzo Biochem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enzo Biochem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Enzo Biochem
provider_slug: enzo-biochem
slug: enzo-biochem-domain-security
source_filename: enzo-biochem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enzo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: enzo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enzo-biochem/refs/heads/main/security/enzo-biochem-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Research Reagents
- Diagnostics
- Drug Discovery
- Immunoassays
- Laboratory
---
