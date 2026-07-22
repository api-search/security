---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: enveda.com
  spf: true
hosts:
- cert_expires: Sep 23 22:03:11 2026 GMT
  host: www.enveda.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enveda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enveda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Enveda
provider_slug: enveda
slug: enveda-domain-security
source_filename: enveda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enveda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:03:11 2026 GMT\n  hsts: false\ndomains:\n- domain: enveda.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enveda/refs/heads/main/security/enveda-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Drug Discovery
- Biotechnology
- Artificial Intelligence
- Machine Learning
- Pharmaceuticals
- Natural Products
---
