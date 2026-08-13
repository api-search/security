---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild ";"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cybcube.com
  spf: true
hosts:
- cert_expires: Sep 27 16:07:03 2026 GMT
  host: www.cybcube.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: api.cybcube.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cybercube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CyberCube, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CyberCube
provider_slug: cybercube
slug: cybercube-domain-security
source_filename: cybercube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cybcube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:07:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cybcube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cybcube.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \";\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybercube/refs/heads/main/security/cybercube-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cyber Risk
- Insurance
- Analytics
- Risk Modeling
- Cybersecurity
- Reinsurance
- Catastrophe Modeling
- Underwriting
- InsurTech
---
