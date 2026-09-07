---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 35pharma.com
  spf: true
hosts:
- cert_expires: Nov 19 01:50:08 2026 GMT
  host: www.35pharma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 35Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 35Pharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 35Pharma
provider_slug: 35pharma
slug: 35pharma-domain-security
source_filename: 35pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.35pharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 01:50:08 2026 GMT\n  hsts: null\ndomains:\n- domain: 35pharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/35pharma/refs/heads/main/security/35pharma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Biopharmaceutical
- Drug Development
- Clinical Trials
- Life Sciences
- Protein Engineering
- Healthcare
---
