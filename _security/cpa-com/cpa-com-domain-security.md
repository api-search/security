---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cpa.com
  spf: true
hosts:
- cert_expires: Feb 22 14:37:57 2027 GMT
  host: www.cpa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cpa Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CPA.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CPA.com
provider_slug: cpa-com
slug: cpa-com-domain-security
source_filename: cpa-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cpa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 14:37:57 2027 GMT\n  hsts: false\ndomains:\n- domain: cpa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cpa-com/refs/heads/main/security/cpa-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Accounting
- Technology
- Advisory
- Community
---
