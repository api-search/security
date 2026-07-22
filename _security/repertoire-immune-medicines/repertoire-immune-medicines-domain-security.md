---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: repertoire.com
  spf: true
hosts:
- cert_expires: Sep  2 02:16:31 2026 GMT
  host: www.repertoire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Repertoire Immune Medicines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Repertoire Immune Medicines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Repertoire Immune Medicines
provider_slug: repertoire-immune-medicines
slug: repertoire-immune-medicines-domain-security
source_filename: repertoire-immune-medicines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.repertoire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:16:31 2026 GMT\n  hsts: false\ndomains:\n- domain: repertoire.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/repertoire-immune-medicines/refs/heads/main/security/repertoire-immune-medicines-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Health Tech
- Biotechnology
- Immunology
- T Cell
- Drug Discovery
- Oncology
---
