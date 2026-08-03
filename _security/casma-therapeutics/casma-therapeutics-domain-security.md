---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: casmatx.com
  spf: true
hosts:
- cert_expires: Aug 25 20:27:40 2026 GMT
  host: www.casmatx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Casma Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Casma Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Casma Therapeutics
provider_slug: casma-therapeutics
slug: casma-therapeutics-domain-security
source_filename: casma-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.casmatx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 20:27:40 2026 GMT\n  hsts: false\ndomains:\n- domain: casmatx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casma-therapeutics/refs/heads/main/security/casma-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Drug Discovery
- Therapeutics
- Autophagy
- Health
---
