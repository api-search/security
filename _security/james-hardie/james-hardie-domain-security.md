---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jameshardie.com
  spf: true
hosts:
- cert_expires: Dec  8 19:19:16 2026 GMT
  host: www.jameshardie.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: James Hardie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for James Hardie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: James Hardie
provider_slug: james-hardie
slug: james-hardie-domain-security
source_filename: james-hardie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jameshardie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 19:19:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jameshardie.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/james-hardie/refs/heads/main/security/james-hardie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Building Products
- Fiber Cement
- Siding
- Construction
- Manufacturing
- Home Improvement
---
