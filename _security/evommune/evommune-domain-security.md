---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: evommune.com
  spf: true
hosts:
- cert_expires: Oct 21 06:37:40 2026 GMT
  host: www.evommune.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evommune Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evommune, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Evommune
provider_slug: evommune
slug: evommune-domain-security
source_filename: evommune-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evommune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 06:37:40 2026 GMT\n  hsts: false\ndomains:\n- domain: evommune.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evommune/refs/heads/main/security/evommune-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Immunology
- Drug Development
- Clinical Trials
- Healthcare
---
