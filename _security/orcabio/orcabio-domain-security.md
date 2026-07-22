---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orcabio.com
  spf: true
hosts:
- cert_expires: Oct  9 13:10:17 2026 GMT
  host: orcabio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orcabio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orca Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Orca Bio
provider_slug: orcabio
slug: orcabio-domain-security
source_filename: orcabio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orcabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:10:17 2026 GMT\n  hsts: false\ndomains:\n- domain: orcabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orcabio/refs/heads/main/security/orcabio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Cell Therapy
- Immunotherapy
- Healthcare
- Life Sciences
- Oncology
---
