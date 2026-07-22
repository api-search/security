---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "godaddy.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amicusrx.com
  spf: true
hosts:
- cert_expires: Oct  9 16:53:30 2026 GMT
  host: www.amicusrx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amicus Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for amicus-therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: amicus-therapeutics
provider_slug: amicus-therapeutics
slug: amicus-therapeutics-domain-security
source_filename: amicus-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amicusrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:53:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amicusrx.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amicus-therapeutics/refs/heads/main/security/amicus-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Pharmaceuticals
- Rare Diseases
- Genetic Diseases
- Fabry Disease
- Pompe Disease
- Lysosomal Storage Disorders
- Enzyme Replacement Therapy
- Pharmacological Chaperones
- Clinical Research
- Life Sciences
- Patient Advocacy
---
