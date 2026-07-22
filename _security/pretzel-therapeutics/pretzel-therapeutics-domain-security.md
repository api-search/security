---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pretzeltx.com
  spf: true
hosts:
- cert_expires: Aug 28 15:26:17 2026 GMT
  host: pretzeltx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pretzel Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pretzel Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pretzel Therapeutics
provider_slug: pretzel-therapeutics
slug: pretzel-therapeutics-domain-security
source_filename: pretzel-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pretzeltx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 15:26:17 2026 GMT\n  hsts: false\ndomains:\n- domain: pretzeltx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pretzel-therapeutics/refs/heads/main/security/pretzel-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Pharmaceuticals
- Therapeutics
- Mitochondrial Medicine
- Drug Discovery
- Rare Disease
---
