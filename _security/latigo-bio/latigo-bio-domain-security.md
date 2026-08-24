---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: latigobio.com
  spf: true
hosts:
- cert_expires: Oct  8 00:20:14 2026 GMT
  host: latigobio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Latigo Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Latigo Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Latigo Bio
provider_slug: latigo-bio
slug: latigo-bio-domain-security
source_filename: latigo-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latigobio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 00:20:14 2026 GMT\n  hsts: false\ndomains:\n- domain: latigobio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/latigo-bio/refs/heads/main/security/latigo-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Drug Discovery
- Clinical Trials
- Healthcare
- Pain Management
- Therapeutics
---
