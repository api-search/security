---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: georgiamune.com
  spf: true
hosts:
- cert_expires: Aug 20 05:15:00 2026 GMT
  host: georgiamune.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Georgiamune Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Georgiamune, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Georgiamune
provider_slug: georgiamune
slug: georgiamune-domain-security
source_filename: georgiamune-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: georgiamune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 05:15:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: georgiamune.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/georgiamune/refs/heads/main/security/georgiamune-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biopharmaceutical
- Immunotherapy
- Oncology
- Autoimmune
- Drug Discovery
- Biotechnology
- Immunology
---
