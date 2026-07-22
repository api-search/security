---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: structuretx.com
  spf: true
hosts:
- cert_expires: Oct 14 18:42:12 2026 GMT
  host: structuretx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Structure Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Structure Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Structure Therapeutics
provider_slug: structure-therapeutics
slug: structure-therapeutics-domain-security
source_filename: structure-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: structuretx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:42:12 2026 GMT\n  hsts: false\ndomains:\n- domain: structuretx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/structure-therapeutics/refs/heads/main/security/structure-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Clinical Trials
- Obesity
- Metabolic Disease
- GLP-1
- GPCR
---
