---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: publicisgroupe.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: publicissapient.com
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: www.publicisgroupe.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: knowhow.suite.publicissapient.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.publicissapient.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Publicis Groupe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Publicis Groupe, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Publicis Groupe
provider_slug: publicis-groupe
slug: publicis-groupe-domain-security
source_filename: publicis-groupe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.publicisgroupe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: knowhow.suite.publicissapient.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.publicissapient.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: publicisgroupe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: publicissapient.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nobservations:\n- host: dev.sapientslingshot.com\n  finding: >-\n    TLS certificate expired. The wildcard *.sapientslingshot.com certificate issued by\n    GoDaddy Secure Certificate\
  \ Authority - G2 ran from 2025-05-09 to 2026-05-09 and was\n    still being served on 2026-09-13, so the host fails default certificate validation.\n    Probed 2026-09-13.\n- host: dev-slingshot.sapientaiproducts.com\n  finding: >-\n    dev.sapientslingshot.com redirects here, and this host answers HTTP 200 with a\n    Prometheus exposition payload (Content-Type text/plain; version=0.0.4) for every path\n    probed, including /, /docs, /health and /openapi.json. It is an unauthenticated\n    metrics endpoint on a development deployment, not an API contract, and no spec was\n    derived from it. Probed 2026-09-13.\n- scope_note: >-\n    Hosts probed by the script are those named in apis.yml. sapientslingshot.com and\n    sapientaiproducts.com are not apis.yml hosts; the two findings above were recorded\n    during contract discovery.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publicis-groupe/refs/heads/main/security/publicis-groupe-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Advertising
- Marketing
- Media
- Digital Transformation
- Consulting
- Artificial Intelligence
- Developer Tools
- Engineering Metrics
- Open Source
- MCP
- Agency Holding Company
---
