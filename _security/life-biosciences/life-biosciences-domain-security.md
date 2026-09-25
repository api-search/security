---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lifebiosciences.com
  spf: true
hosts:
- cert_expires: Sep 19 11:45:04 2026 GMT
  host: www.lifebiosciences.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Life Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Life Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Life Biosciences
provider_slug: life-biosciences
slug: life-biosciences-domain-security
source_filename: life-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lifebiosciences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:45:04 2026 GMT\n  hsts: false\ndomains:\n- domain: lifebiosciences.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/life-biosciences/refs/heads/main/security/life-biosciences-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Longevity
- Aging
- Gene Therapy
- Ophthalmology
- Content
---
