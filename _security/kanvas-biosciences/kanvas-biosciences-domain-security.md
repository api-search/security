---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kanvasbio.com
  spf: true
hosts:
- cert_expires: Sep 14 09:22:14 2026 GMT
  host: www.kanvasbio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kanvas Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kanvas Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kanvas Biosciences
provider_slug: kanvas-biosciences
slug: kanvas-biosciences-domain-security
source_filename: kanvas-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kanvasbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:22:14 2026 GMT\n  hsts: null\ndomains:\n- domain: kanvasbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kanvas-biosciences/refs/heads/main/security/kanvas-biosciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Microbiome
- Spatial Biology
- Drug Discovery
- Immuno-Oncology
- Therapeutics
---
