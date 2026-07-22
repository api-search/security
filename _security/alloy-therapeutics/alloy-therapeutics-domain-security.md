---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: alloytx.com
  spf: true
hosts:
- cert_expires: Oct  1 10:01:00 2026 GMT
  host: alloytx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alloy Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alloy Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Alloy Therapeutics
provider_slug: alloy-therapeutics
slug: alloy-therapeutics-domain-security
source_filename: alloy-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alloytx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:01:00 2026 GMT\n  hsts: false\ndomains:\n- domain: alloytx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy-therapeutics/refs/heads/main/security/alloy-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Drug Discovery
- Antibody Discovery
- Genetic Medicines
- Artificial Intelligence
- Life Sciences
- Pharmaceutical
---
