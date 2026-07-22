---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leydenlabs.com
  spf: true
hosts:
- cert_expires: Sep  8 19:28:50 2026 GMT
  host: leydenlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leyden Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leyden Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Leyden Labs
provider_slug: leyden-labs
slug: leyden-labs-domain-security
source_filename: leyden-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leydenlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 19:28:50 2026 GMT\n  hsts: false\ndomains:\n- domain: leydenlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leyden-labs/refs/heads/main/security/leyden-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Pharmaceuticals
- Immunology
- Infectious Disease
- Vaccines
- Antibodies
- Respiratory Health
- Clinical Trials
- Netherlands
---
