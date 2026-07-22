---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: drenbio.com
  spf: true
hosts:
- cert_expires: Sep 23 12:22:35 2026 GMT
  host: drenbio.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dren Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dren Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dren Bio
provider_slug: dren-bio
slug: dren-bio-domain-security
source_filename: dren-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drenbio.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 12:22:35 2026 GMT\n  hsts: false\ndomains:\n- domain: drenbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dren-bio/refs/heads/main/security/dren-bio-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Biopharmaceutical
- Biotechnology
- Antibody Therapeutics
- Oncology
- Autoimmune
- Immunology
- Neurology
- Drug Development
---
