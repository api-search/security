---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boundlessbio.com
  spf: true
hosts:
- cert_expires: Sep 13 01:31:53 2026 GMT
  host: boundlessbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boundless Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boundless Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boundless Bio
provider_slug: boundless-bio
slug: boundless-bio-domain-security
source_filename: boundless-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boundlessbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 01:31:53 2026 GMT\n  hsts: false\ndomains:\n- domain: boundlessbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boundless-bio/refs/heads/main/security/boundless-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Oncology
- Precision Medicine
- Drug Discovery
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Genomics
- Diagnostics
- Research
- Content
---
