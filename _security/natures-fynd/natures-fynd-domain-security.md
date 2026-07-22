---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: naturesfynd.com
  spf: true
hosts:
- cert_expires: Aug 31 10:55:25 2026 GMT
  host: www.naturesfynd.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Natures Fynd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nature''s Fynd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nature's Fynd
provider_slug: natures-fynd
slug: natures-fynd-domain-security
source_filename: natures-fynd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.naturesfynd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:55:25 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: naturesfynd.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natures-fynd/refs/heads/main/security/natures-fynd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Food
- Biotechnology
- Fermentation
- Alternative Protein
- Manufacturing
---
