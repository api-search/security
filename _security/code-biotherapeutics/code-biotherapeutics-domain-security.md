---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: codebiotx.com
  spf: true
hosts:
- cert_expires: Sep  4 12:40:12 2026 GMT
  host: www.codebiotx.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Code Biotherapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Code Biotherapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Code Biotherapeutics
provider_slug: code-biotherapeutics
slug: code-biotherapeutics-domain-security
source_filename: code-biotherapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codebiotx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 12:40:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: codebiotx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/code-biotherapeutics/refs/heads/main/security/code-biotherapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Genetic Medicine
- Gene Therapy
- Life Sciences
- Pharmaceuticals
- Rare Disease
- Drug Discovery
---
